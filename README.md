# Toxic_comment_classification
Multilabel Text Classification model using pretrained BERT base-uncased model

Problem Statement:
Given a dataset of comments, the task is to classify them based upon the context of the words. There are 6 classes; toxic, severe_toxic, obscene, threat, insult, identity_hate.

The problem was solved using the followed algorithms and the following highest accuracies were achieved :
1. BERT : 93%
2. LSTM : 91.8%
3. CNN : 90.68%

BERT (Bidirectional Encoder Representations from Transformers):
BERT is the first deeply bidirectional, unsupervised language representation, pre-trained using only a plain text corpus. BERT makes use of Transformer, an attention mechanism that learns contextual relations between words (or sub-words) in a text. In its vanilla form, Transformer includes two separate mechanisms — an encoder that reads the text input and a decoder that produces a prediction for the task. As opposed to directional models, which read the text input sequentially (left-to-right or right-to-left), the Transformer encoder reads the entire sequence of words at once. Therefore, it is considered bidirectional, though it would be more accurate to say that it’s non-directional. This characteristic allows the model to learn the context of a word based on all of its surroundings (left and right of the word). Context-free models such as word2vec or GloVe generate a single word embedding representation for each word in the vocabulary. Contextual models instead generate a representation of each word that is based on the other words in the sentence. Contextual representations can further be unidirectional or bidirectional. Multi-class classification & Multi-label classification: Difference between multi-class classification & multi-label classification is that in multi-class problems the classes are mutually exclusive, whereas for multi-label problems each label represents a different classification task, but the tasks are somehow related.

LSTM (Long Short-term memory):
Long Short Term Memory networks – usually just called “LSTMs” – are a special kind of RNN, capable of learning long-term dependencies.They work tremendously well on a large variety of problems, and are now widely used. LSTMs are explicitly designed to avoid the long-term dependency problem. Remembering information for long periods of time is practically their default behavior, not something they struggle to learn.

CNN (Concurrent Neural Networks):
Convolutional Neural Networks have been revolutionary in the field of Deep Neural Networks, and have
changed the dynamics of applications in Image Processing and Computer Vision. ConvNets consist of two
types of layers added to the traditional fully connected neural nets, namely “Convolution” and “Pooling”.
A kernel or convolutional filter is mapped over the channel dimensions consisting of local features of the
samples, while the max-pooling layer reduces dimensions of the convolved feature maps to be given as
inputs to the subsequent layers. This combination, on top of a pre-trained model for word vector
generation, while tuning hyper-parameters has provided some considerable results. The convolutional
layers extract key features from the data, which is then fed to a Fully Connected Layer or Dense Neural
Net layer, to perform the final classification.
