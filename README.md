# Is a RNN based deep neural network application used to classify spam messages using NLP

Dataset    : [Dataset](https://www.kaggle.com/team-ai/spam-text-message-classification)<br/>
Framework  : [Tensorflow v2.x](https://www.tensorflow.org/)<br/>
#Training  : 5014<br/>
#Testing   : 558<br/>

## Word embedding used : [Glove 300d](https://nlp.stanford.edu/projects/glove/)

## Architecture : <br/>

**Layer 1** : Input layer<br/>
**Layer 2** : Embedding layer<br/>

**Layer 3** : LSTM (units=128)<br/>
**Layer 4** : Dropout(rate=0.2) 

**Layer 5** : LSTM(units=128)<br/>
**Layer 6** : Dropout(rate=0.2)<br/>

**Layer 7** : Dense(5, activation= Relu)<br/>
**Layer 8** : Dense(1, activation= Relu)<br/>
**Layer 9** : Sigmoid()<br/>

**Cost Function** : Binary Cross entropy<br/>
**Optimization** : Adam's Optimization<br/>

| Epochs       | Train Accuracy           | Test Accuracy  | Train Loss |
| ------------- |:-------------:| -----:| -----------:|
| 3 | 0.8566      |    0.8670 | 0.3942 |

**Increasing epochs or decreasing the dropout rate doesn't seem to increase the accuracy of neither training or testing**

    
