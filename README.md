# Youtube_comments_sentiment_analysis_NLP
 
**Summary:** Sentiment analysis is one of the main methods in NLP (Natural Language Processing). Focusing on one of my favorite YouTube channels -- Outdoors Chef Life (https://www.youtube.com/@OutdoorChefLife), this project uses sentiment analysis to analyze the changes in comment polarity for 300+ videos and their comments. Polarity is a measurement of how positive the language is -- 1 means very positive, 0 means neutral, and -1 means negative comments. I then analyzed and visualized the comment polarity by plotting the comment polarity from the oldest video to the latest video, showing the temporal changes in the polarity of Youtube comments across the channel's Youtube history. I also produced a word cloud image based on the video with the highest polarity score (most positive) on its comments. 


**Data source:** YouTube comments extracted from the videos of the channel (https://www.youtube.com/@OutdoorChefLife). 


**Repository structure:**
01_Codes: storing jupyter notebook of python codes. "Youtube_comment_sentiment_analysis_single_video" analyzes one YouTube video using sentiment analysis and produces word-cloud image of the comments from that video. "Youtube_comment_sentiment_analysis_multiple_video" analyzes all 300+ videos by using the loop function, it then produces an interactive Plotly plot to help visualize and track changes in comment polarity across the publication history of the Youtube channel. 


**Installation Required:**

Python3

import itertools 

from youtube_comment_downloader import *

import re

import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

from IPython.core.interactiveshell import InteractiveShell
InteractiveShell.ast_node_interactivity = "all"

#NLP packages
from textblob import TextBlob

from nltk.corpus import stopwords

from wordcloud import WordCloud, STOPWORDS

import spacy

import nltk


**Data visualization:**
![image](https://github.com/YingtongAamandaWu/Youtube_comments_sentiment_analysis_NLP/assets/80353259/ff5eb654-e850-4786-978d-423b1923f131)

![image](https://github.com/YingtongAamandaWu/Youtube_comments_sentiment_analysis_NLP/assets/80353259/fe4f7434-6782-4a70-8ff0-48274ad1f857)
