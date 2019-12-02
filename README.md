# Miquela Video Comment Analysis
![Miquela](ss2.jpg)


### data_preprocessing+model.ipynb 
Load data
LDA Model 
Sentiment Analysis

### downloader.py
Simple script for downloading Youtube comments without using the Youtube API. The output is in line delimited JSON.

#### downloader.py Usage
```
usage: downloader.py [--help] [--youtubeid YOUTUBEID] [--output OUTPUT]

Download Youtube comments without using the Youtube API

optional arguments:
  --help, -h            Show this help message and exit
  --youtubeid YOUTUBEID, -y YOUTUBEID
                        ID of Youtube video for which to download the comments
  --output OUTPUT, -o OUTPUT
                        Output filename (output format is line delimited JSON)
```
### data -- youtube comments in json format
### lda_model -- saved gensim lda model
