# DisasterTweets
![Real or Not? NLP with Disaster Tweets](https://www.kaggle.com/c/nlp-getting-started)

<cite>Twitter has become an important communication channel in times of emergency.
The ubiquitousness of smartphones enables people to announce an emergency they’re observing in real-time. Because of this, more agencies are interested in programatically monitoring Twitter (i.e. disaster relief organizations and news agencies).</cite>

For example:
**A tweet about real emergency**
_text_
> My last two weather pics from the storm on August 2nd. People packed up real fast after the temp dropped and winds picked up.
_keyword_
> storm
_location_
> Ottawa, Ontario

**A tweet about non-emergency**
_text_
> That sounds about right. Our building will have a thunderstorm inside one day when the air masses collide. https://t.co/2rTQ9QmGPB
_keyword_
> collide
_location_
> Kansas, The Free State! ~ KC

## Description
This notebook, [**DisasterTweets.ipynb**](/NLP-with-Disaster-Tweets/blob/master/DisasterTweets.ipynb), is a short demonstration of applying the Bidirectional Encoder Representations from Transformers (BERT) from tensorflow hub for learning purposes. An natural language processing (NLP) model is built to predict if a given tweet is talking about a real emergency situation or not. The data comes from a kaggle competition at "getting started" level, see [Real or Not? NLP with Disaster Tweets](https://www.kaggle.com/c/nlp-getting-started).

[**DisasterTweets.ipynb**](/NLP-with-Disaster-Tweets/blob/master/DisasterTweets.ipynb) studies three approaches. The first solution is to finetune BERT from pretrained weights in a few epochs of training. The second solution is to attach more dense layers after BERT while freezing BERT's weights. This way of transfer learning complexifies the model's structure for broader missions without heavy retraining. Finally, the third solution explores more models attached after BERT to further improve the predictions.

## Content
The content in [**DisasterTweets.ipynb**](/NLP-with-Disaster-Tweets/blob/master/DisasterTweets.ipynb) includes the following.
0. Outline
1. minimum data exploration and preprocessing
2. finetune a pretrained BERT model
3. transfer learning with BERT
4. subsequent booster after BERT

## How to run it
One can run [**DisasterTweets.ipynb**](/NLP-with-Disaster-Tweets/DisasterTweets.ipynb) on google's colab with runtime type set to GPU/Python 3, or simply click ![colab link](https://drive.google.com/open?id=1OQprbW062EJFKmBHQNlLzqdGICJVOi5w).
All dataset, modules, and models will be downloaded and installed on colab. Readers are encouraged to tune parameters and implement different models for learning purposes.

## Author
* Ken Yeh, <kenyeh@matrixdata.club>
## Dataset
[**train.csv**], [**test.csv**], [**sample_submission.csv**]
The training data in this project belongs to [Florence 2D/3D Face Dataset](http://www.micc.unifi.it/masi/research/ffd/) by Bagdanov, Andrew D. and Masi, Iacopo and Del Bimbo, Alberto, MICC-University of Florence. The author is grateful to Prof. Stefano Berretti for his assistance with data acquisition.
