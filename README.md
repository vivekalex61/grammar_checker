
# Grammar checker

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)

Trained a Transformer model called T5 to solve grammar mistakes
## Introduction 

#### Grammar correction
Grammar correction is a common task in NLP. Perhaps you want to provide recommendations to our users to improve their writing, or maybe we want to improve the quality of your training data. In either case, we can use the model we're about to describe.




## Overview 
- Datasets and Data-Loading
- Data Preprocessing
- Model creation

### Datasets and Data-Loading

JFLEG (JHU FLuency-Extended GUG) is an English grammatical error correction (GEC) corpus. It is a gold standard benchmark for developing and evaluating GEC systems with respect to fluency (extent to which a text is native-sounding) as well as grammaticality. For each source document, there are four human-written corrections.

link : https://huggingface.co/datasets/jfleg

Sample: 

![alt text](https://raw.githubusercontent.com/vivekalex61/grammar_checker/main/images/dataset%20samples.png)



### Data Preprocessing
 Preprocessing of data includes 
 
1)Removing unwanted symbols and values




### Model building and training





#### 1)T5 transformer

T5, or Text-to-Text Transfer Transformer, is a Transformer based architecture that uses a text-to-text approach. Every task – including translation, question answering, and classification – is cast as feeding the model text as input and training it to generate some target text. This allows for the use of the same model, loss function, hyperparameters, etc. across our diverse set of tasks. The changes compared to BERT include:

1,adding a causal decoder to the bidirectional architecture.

2,replacing the fill-in-the-blank cloze task with a mix of alternative pre-training tasks.



![alt text](https://raw.githubusercontent.com/vivekalex61/grammar_checker/main/images/t5.jpg)


#### Training

1)Tokenizing texts using T5 tokenizer

2)Configuring the model

3)Train model


## Results
Below are the results  got from trained transformer.
![alt text](https://raw.githubusercontent.com/vivekalex61/insightsearch/master/test/overall_sentiments.png)


## End Notes

The model is not finetuned .
