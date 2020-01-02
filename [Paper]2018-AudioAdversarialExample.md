# Audio Adversarial Examples: Targeted Attacks on Speech-to-Text

**Authors:** Nicholas Carlini David Wagner

University of California, Berekley

**Link:** https://arxiv.org/pdf/1801.01944.pdf

**Year:** 2018

**Codebase:** http://nicholas.carlini.com/code/audio adversarial examples

**Overview:**
- Constructed audio adversarial examples to attack [DeepSpeech](https://github.com/mozilla/DeepSpeech), which is used for automatic speech recognition
- Finds that adding a small pertubation to the audio waveform changes the transcribed result. The pertubation is not audible to the human ear.

**Threat Model:** 
- Given an audio waveform x, and target tran- scription y, our task is to construct another audio waveform $x′ = x + δ$ so that $x$ and $x′$ sound similar, but so that $C(x′) = y$. 
- Dataset: [Common Voice test set](https://voice.mozilla.org/en/datasets)

**Experiments:**
- Distortion metric: distortion in dB. Perturbation is quieter than original signal.
- Loss Function impacts the final distortion of generated adversarial examples. Constructed an improved loss function to optimise the transcribed phrase.
- Starting from non-speech (classical music) + target phrases in Common Voice Dataset works too, except total distortion is slightly larger and more computational effort required
- Targeting silence: hide speech by adding adversarial noise that causes DeepSpeech to transcribe nothing.with distortion less than −45dB below the original signal, we can turn any phrase into silence.
This partially explains why it is easier to construct adver- sarial examples when starting with longer audio waveforms than shorter ones: because the longer phrase contains more sounds, the adversary can silence the ones that are not required and obtain a subsequence that nearly matches the target. In contrast, for a shorter phrase, the adversary must synthesize new characters that did not exist previously.
- When plotted, original waveform and adversarial waveform are impossible to notice a difference as they overlay each other
- Audio Information Density: Input waveform is converted into 50 frames per second of audio, and DeepSpeech outputs one probability distribution of characters per frame, so theoretical maximum density of audio is 50 characters per second, that can be generated. The logit-based loss function can be applied directly without first finding an alignment

**Open Questions:**
- Ideas the authors have for further work in the paper: 
- Can these attacks be played over-the-air? 
- Do universal adversarial perturbations exit?
- Are audio adversarial examples transferable?
- Which existing defences can be applied to audio? 

**Other notes:**
- Neural networks are vulnerable to adversarial examples: instances *x'* similar to natural instance *x* but classified by neural network as incorrect target *t* chosen by the adversary.
- Existing work on adversarial examples are focused largely on the space of images, and comparatively little study in audio, where the most common use is performing automatic speech recognition. In automatic speech recognition, a neural network is given an audio waveform *x* and perform the speech-to-text transform that gives the transcription *y* of the phrase being spoken
- Difficulty of producing adversarial examples: hidden and inaudible voice commands are targeted attacks, require synthesising new audio and not modify existing audio. SOTA attack is [Houdini](https://arxiv.org/abs/1707.05373).  Other work has constructed standard untargeted adversarial examples on different audio systems.
- [Connectionist Temporal Classification](https://www.cs.toronto.edu/~graves/icml_2006.pdf) is a method of training a sequence to sequence neural network when the alignment between the input and output sequences is not known. 
