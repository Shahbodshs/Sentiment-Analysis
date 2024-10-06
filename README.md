# Sentiment-Analysis
In this repository you can have access to the code file of a sentiment analysis project. 

## Explanations about the codes: 
The project hasn't done specifically by me, i just studied a source code from kaggle but i changed a few things about the code.
the source : [Sentiment analysis with BILSTM](https://www.kaggle.com/code/stoicstatic/twitter-sentiment-analysis-using-word2vec-bilstm/notebook).
## Changes from the source code : 
1. Preprocessing part of the code :
the first thing i changed from the code is the preprocessing part, where i believe replacing  the contractions form of a word to original format like : __can't__ to __can not__ is wrong and not every user in real life type like this so the model has to actually learn from these too since we are working with BILSTMs the model is totally capable of learning it. 
i have also changed the part where the user tried to remove the non alphabetic words and emojies for the same reason. 
but just like the source code i still removed the url and user tags because they are actually considered as noises. 
2. Vocab size: 
i have also changed the size of the vocab sze to 90k since the vocab size after not removing non alphabetic characters and emojies caused much larger vocab length. 
but the model could also get improved but it needed to analyse the whole vocab which i was not capable of doing it(takes a huge amount of time and resource). 


The whole reason of doing this was to do a personal project for my resume, i hope you have enjoyed reviewing the code as well as i did.

# The dataset source : 
[Sentiment140](https://www.kaggle.com/datasets/kazanova/sentiment140)    


## You can have access to the code in the __code__ branch.


# Updates about the project: 
I am considering to make some changes in the future in the model. 
in the  last lines you might see that the validation loss starts to increase while the train set loss still decreasing. 
i will implement early stopping and evaluate the validation test at the same time for each epoch. 
also im considering to create another SA model but using a [Transformer](https://huggingface.co/learn/nlp-course/en/chapter1/1?fw=pt) model. 


## Update 1:
I have created a better model with mre accuracy, but it still has potential for improvements, but the file having the name update-1 is the newer version for now. 
