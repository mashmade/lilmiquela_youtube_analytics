Since I wrote the paper in 2018,  Miquela has expanded into becoming a vlogger and musician as well and has posted such content on YouTube. In an effort to understand how people feel about an AI celebrity/star, I analyzed the comments on one of her music video titled: “Miquela- Automatic”, with 2.1 million views. By  levarging natural language processing techniques I was able to clean webscraped youtube comments data for emojis, punctuation, and stop words. The clean data was analyzed using two methods. First the data was processed through a Latent Direchlec Allcoaiton model, using python package Gensim, to see if comment content could be separated into distinct n clusters. It was noticed that certain topics related to excitiment, awe, love and interest had distinct clusters,  while other topics had heavily weighted terms related to fear, confusion and suspicison.
Secondly, these clusters and raw comments were then evaluated for sentiment and objectivity metrics using Textblob; polarity (-1 being negative , +1 being postive) and subjectivity (0 being factual and 1 being subjective). A goal of mine is to create a pipline that is continously deployed and extracts data on new comments, from existing and new video uploads automatically. This data could be visualized over time, and correlated with novel developments in the field, as an insight to public perception of Artifical Intellgience by a particular demographic. My data analysis and visualization can be found below:


# downloader.py
Simple script for downloading Youtube comments without using the Youtube API. The output is in line delimited JSON.

### Usage
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
