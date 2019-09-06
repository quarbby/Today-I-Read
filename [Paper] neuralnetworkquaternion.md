# Lightweight and Efficient Neural Natural Language Processing with Quaternion Networks 

Authors: Yi Tay, Aston Zhang, Luu Anh Tuan, Jinfeng Rao, Shuai Zhang, Shuohang Wang, Jie Fu, Siu Cheung Hui

Link: https://arxiv.org/pdf/1906.04393.pdf

**Overview**

Paper introuduced two novel methods: (1) Quaternion Attention Model and (2) Quaternion Transformer.

These are similar to the current Attention Models (https://medium.com/@joealato/attention-in-nlp-734c6fa9d983) and Transformer models (https://www.analyticsvidhya.com/blog/2019/06/understanding-transformers-nlp-state-of-the-art-models/). The paper improved the models by introeducing Quaternion variants of the models, which reduces parameter size due to lesser degrees of freedom in the Hamilton product, because Quaternion spaces explictly encodes latent interactions between components by the Hamilton product. 

**Contributions**

Many dominant neural architectures have millions of parameters that render deployment and training challenging. This method reduces the number of variables by about half.

**Drawbacks**

The accuracy of the NLP tasks experimented on increased from 82% in the baseline Transformer model to 83% using quaternion architecture, hence giving little reason to adopt this model for operations use.

**Code**

Code is available on Github in Tensorflow implementation: https://github.com/ vanzytay/QuaternionTransformers. 

