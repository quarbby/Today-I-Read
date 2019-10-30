## Cognitively Inspired Natural Language Processing/ An Investigation Based on Eye-tracking
By Abhijit Mishra and Pushpak Bhattacharyya

[Link to Book](https://www.springer.com/us/book/9789811315152)

* Text is a manifestation of thought and emotion that give rise to cognitive processes in the brain. When a reader reads a piece of text, she experiences emotions, stances, nuances, subtleties, inferences, suggestions and much more.
* The goal of NLP, or Computational Linguistics, is to translate linguistic principles and artifacts to and fro computer-understandable forms.
* Several layers of language processing activities: 
  * Lexical analysis: phonology, morphological analysis
  * Syntactic Analysis: part-of-speech tagging and syntactic parsing
  * Semantic Analysis: semantic role inference
  * Discourse analysis and pragmatics: discourse parsing, co-reference resolution, detection of sentiment and emotional content in text
* Types of cognitive data:
  * Gaze data
    * Gaze points: Position of eye-gaze on the screen
    * Fixation: How long of the gaze on an object on the screen. Spatial (coordinates) and temporal (duration) dimensions
    * Saccade: Very rapid movement of eyes between positions of rest
    * Scanpath: Line graph that contains fixation as nodes and saccades as edges. It may be convenient to analyse/compare scanpaths, if a metric for mathematically comparing similarity between two scanpaths may be proposed.
      * Fixation Attributes: total fixation duration, first-fixation duration, regressive-fixation duration, fixation count, skipper word
      * Saccadic Attributes: regression count, saccadic distance, regression distance, negative saccade log likelihood
      * Future work: individual factors (e.g. age, domain expertise, language skills), joint model of fixations and saccades for scanpath complexity measurements
  * Keystroke data
    * Insertion of word/char inside running text
    * Deletion
    * Selection/ highlighting
    * Rearrangement of piece of text
* Example of cognitive data in annotation: 
  * Visualisation: viewing the raw data on a monitor screen
  * Comprehension: understanding the data
  * Generation: assigning the appropriate annotation labels to the data 
* The landing of the eye may seem random, but it relates to the memory, expectations and goals of the viewer.
* Eye tracking technologies: electro-oculography, scleral search coils, infrared oculography, video-oculography
* Eye movement in reading and language processing
  * The hypothesis is that when a subject views a word/object, he or she is also processing it cognitively, for approximately the same amount of time he or she fixates on it. 
  * Gaze patterns indicate conceptual difficulty the reader experiences. Linear/ uniform speed gaze movement observed with texts with simple concepts.
    * Basic gaze features: average first-fixation duration per word, average fixation count, average saccade length, regression count, skip count, count of regressions from second half to first half of sentence, largest regression position
    * Complex gaze features: edge density of saliency-gaze graph, fixation duration at left/source as edge weight, forward saccade distance as edge weight, regressive saccade count
* Measuring Complexity
  * Text Translation Complexity: Translation Complexity Index with properties of input sentence
    * Lexical features: sentence length, degree of polysemy, out of vocabulary measure, fraction of nouns/ verbs/ preposition, presence of digits, named entity count, average syllabus per word
    * Syntactic features: structural complexity, non-terminal to terminal ratio
    * Semantic features: co-reference distance, passive clause count, discourse connectors count, height of hypernymy, perplexity
    * Translation model entropy
  * Sentiment Annotation Complexity: linguistic features 
    * Lexical: length, polysemy, mean word length, percentage of nouns/ adjectives, percentage of out of vocabulary words
    * Syntactic: Lin structural complexity, non-terminal to terminal ratio
    * Semantic: discourse connectors, perplexity, co-reference distance
    * Sentiment related: Subjective word count, subjective score count, sentiment flip count
* Major processes in reading comprehension by Just and Carpenter (1980):
  * Working Memory: activated representations, physical features, words, meanings, case-roles, clauses, text units, domains of discourse
  * Long Term Memory: orthography, phonology, syntax, semantics, pragmatics, discourse structure, domain knowledge, episodic knowledge
 
