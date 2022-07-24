# WERATEDOGS Data Wrangling Project
## by Keith Obade


## Dataset

I obtained the twitter master dataset from the cleaning process that I had done. This gave me a chance to assess it and look for some insights from the combined twitter master dataset on the WeRateDogs information. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog.

I had three datasets to wrangle. These were the image prediction, twitter enhanced archive csv and the additional data from twitter. The data wrangling process involves three steps; gathering, assessing and cleaning the data. This is to be done so that I can be able to have a dataset I can be able to get correct insights from.

The dataset I am wrangling is the tweet archive of Twitter User @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog.

The archive contains basic tweet data for tweets as at August 1,2017.

Therefore, the first step was to gather the data we want. I used three methods, getting;

    - The twitter_enhanced_archive through direct download.
    - The image prediction file from the udacity server through a url.
    - Additional twitter information from the Twitter API.

From these three processes, I was able to obtain three files with the Twitter API additional data being the hardest since it was a new experience having the developer account to using keys and having to use new functions and modules. With the twitter enhanced dataset, it was simply downloading the file and the image prediction file was obtainable using the request module and then saving it on my local computer.

After gathering the datasets, I then needed to assess them to get the quality and tidiness issues through both visual and programmatic assessment. I opened all files and visually assessed them and got some few issues. I also used some functions to assess it programatically and also got other data issues. Below are the quality and tidiness issues I got:

### Quality issues
#### Twitter archive data

    1. Wrong datatype with pieces of data.
    2. There are retweets in the dataframe.
    3. Name column contains non valid names.
    4. Source column is a link are not categories.
    5. Unnecessary columns.
    6. Source column is duplicated in the tweet json and twitter archive file.
    7. Rating numerator is not float and has wrong values.

#### Json data

    1. The id column not similar to the other dataframes.

#### Image predictions data

    1. p1, p2 and p3 columns data inconsistent: underscored.

#### Tidiness issues

    1. Some expanded urls have multiple variables i.e: links.
    2. Clean the doggo, floofer, pupper, puppo columns in twitter archive data frame.
    3. Merging the datasets.

After obtaining the issues, I went on to tackle them one by one programmatically through the cleaning stage. In the cleaning stage I used the method of: Define, Code and Test. This allowed me to define the action I was taking to clean the issue, code through then test if it changed. All data issues were solved and I merged the datasets so that I can be able to analyze the dataset as one dataframe.

## Insights

Below are the questions I got from assessing the dataset:

    - Which source has the highest number of tweets?
    - Which tweets were the users most favorite and what ratings do they have?
    - What are the most common vs rare dog names?



## Key Insights for Presentation


### Which source has the highest number of tweets?

This question was brought about by observing the source column on the data set and observing that there are 4 main categories of the source of the tweets. Therefore, the question arose on which source could have the highest number of tweets. From the figure below, I observed that the source that had the highest number of tweets was from Iphone with 2042 tweets while the lowest is Tweet Deck with 11.

### Which tweets were the users most favorite and what ratings do they have?

I then went on to look at the top 10 favorite tweets of the data set and what was the most common rating among them. From the analysis, I observed that the most favourite tweet had a count of 132810. Among the top 10 most favorite tweets, the most frequent rating was 13.

### What are the most common vs rare dog names?

The final question was about which dog names were versus the rare names. From the analysis of the names, I observed that the most common names were Charlie, Lucy, Cooper, Oliver and Penny were the most common while there were numerous names that were used only once with Charlie and Lucy appearing 11 times.

## Conclusions

1. I observed that the source that had the highest number of tweets was from Iphone with 2042 tweets while the lowest is Tweet Deck with 11.
2. I observed that the most favourite tweet had a count of 132810. Among the top 10 most favorite tweets, the most frequent rating was 13.
3. I observed that the most common names were Charlie, Lucy, Cooper, Oliver and Penny were the most common while there were numerous names that were used only once with Charlie and Lucy appearing 11 times.

## Limitations

1. I did not perform statistical tests on the data frame provided.

2. I used the dataset with some missing values.
