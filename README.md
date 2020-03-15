## SUMMARY
The focus of this project was primarily on data wrangling. I have executed the whole process from Data Gathering, Wrangling to Analysis and Visualisation. 

The insights from this projects are:
<ol>
  <li> The most liked dog stage on WeRateDogs account was unsurprisingly puppies. Everybody loves puppies and their average favorite count is off the charts. </li>
  <li> Surprisingly, the top 10 dogs with the most follower count are not that far from each other and all have over 8.681 million followers.</li>
  <li> The highest rated dog is Atticus who clearly dominates the scoring. Although one might be concerned by the bias of the evaluator, given that the Atticus has an all american look. </li>
</ol>

## INTRODUCTION
There are 3 sources that have been used for this data analysis:
<ol>
  <li> WeRateDogs dataset that has been exclusively given to Udacity for this project in the form of a csv file. The name of that dataset is twitter_archive. It contains over 5000 tweets as of 1st of August 2017. I downloaded this dataset and accessed it in the jupyter notebook. </li>
  <li> The second dataset was image_tweets which is dataset of predictions using convolutional neural network on the images of the dogs to classify them into their breeds. I programmatically downloaded this dataset using request Python library and downloaded it as a tsv file </li>
  <li> Lastly, using tweet IDs from the twitter_archive (our first dataset), I queried the Twitter API to get each tweet´s data in JSON format. For that I used a Tweepy library. I stored each tweet´s entire data that were later further processed </li>
</ol>

## QUESTIONS INVESTIGATED
<ol>
  <li> What stage of dogs has the most favorites(likes)? In other words, which dog stage seems to be most liked? </li>
  <li> What are the top 10 dogs with the highest number of followers? </li>
  <li> Using the first prediction, what are the top 10 dog breeds with the highest rating </li>
</ol>

## PROCESS OUTLINE
Data Gathering
<ol>
  <li> WeRateDogs main datasets was available in Udacity so I downloaded that and accessed it from the jupyter notebook </li>
  <li> Image_tweets I programmatically downloaded using request Python library </li>
  <li> For detailed twitter information, I queried Twitter API using Tweepz library. </li>
</ol>

Once all the datasets were available, I investigated the dataset using both visual and programmatic assessment.

Visual Assessment
I printed the heads (first five rows) and tails (last five rows) of each dataset to observe clean discrepancies in data quality or tidiness.

Programmatic Assessment
I used a variety of pandas methods such as:
.info()
.value_counts()
.isnull().sum()
.duplicated()
.groupby()

Afterwards I have written down and categorized issues into data quality or data tidiness depending on the character of the problem at hand and cleaned the data and merged these datasets into one file.

Then, I briefly analysed and visualised the data to answer the questions that I asked at the beginning of the data exploration process.
