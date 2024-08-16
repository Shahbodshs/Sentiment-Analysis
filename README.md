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
