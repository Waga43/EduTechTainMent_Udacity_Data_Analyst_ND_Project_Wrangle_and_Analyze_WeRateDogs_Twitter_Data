# EduTechTainMent_Udacity_Data_Analyst_ND_Project_Wrangling_and_Analyze_WeRateDogs_Data
Data wrangling and Analysis of the Twitter WeRateDogs dataset

# Project: Wrangling and Analyze Data
## Project Background

### Background Information

**Information From the Udacity website:**

> The dataset that you will be wrangling (and analyzing and visualizing) is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.


> **Context**


>**Your goal**: 
Wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations. The Twitter archive is great, but it only contains very basic tweet information. Additional gathering, then assessing and cleaning is required for "Wow!"-worthy analyses and visualizations.

> **The Data**


>In this project, you will work on the following three datasets.

> 1. ***Enhanced Twitter Archive***

> ***The WeRateDogs Twitter archive*** contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, which I used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced." Of the 5000+ tweets, I have filtered for tweets with ratings only (there are 2356).

> I extracted this data programmatically, but I didn't do a very good job. The ratings probably aren't all correct. Same goes for the dog names and probably dog stages (see below for more information on these) too. You'll need to assess and clean these columns if you want to use them for analysis and visualization.

> 2. ***Additional Data via the Twitter API***

> Back to the basic-ness of Twitter archives: retweet count and favorite count are two of the notable column omissions. Fortunately, this additional data can be gathered by anyone from Twitter's API. Well, "anyone" who has access to data for the 3000 most recent tweets, at least. But you, because you have the WeRateDogs Twitter archive and specifically the tweet IDs within it, can gather this data for all 5000+. And guess what? You're going to query Twitter's API to gather this valuable data.

> 3. **Image Predictions File**

> One more cool thing: I ran every image in the WeRateDogs Twitter archive through a neural network that can classify breeds of dogs*. The results: a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images).

**Explanation of the Column Names**

According to the Twitter documentation (Data Dictionary: Standard v1.1):

- `ID` refers to the tweet ID which is the integer representation of the uniqueidentifier of this tweet. Using a signed 64bit integer for storing this identifier is said to be safe.


- `retweet_count` An integer which refers to the number of times a tweet has been ***retweeted***.

- `favorite_count` also an integer and indicates approximately how many times a tweet has been ***liked*** by twitter users.

- `text` refers to the actual UTF-8 text of the status update.

- `source` Refers to the tweet post, as an HTML formatted string.

- `in_reply_to_status-id` If the represented tweet is a reply, this entry is an integer that refers to the original tweet's ID.

- `in_reply_to_user_id` If the represented tweet is a reply, this field will contain the integer representation of the oroginal Tweet's author ID.

---

To read the complete report of all the wrangling and analysis of this WeRateDogs Twitter dataset, please refer to the following files:

1. [Data Wrangling Notebook](https://github.com/Waga43/EduTechTainMent_Udacity_Data_Analyst_ND_Project_Wrangle_and_Analyze_WeRateDogs_Twitter_Data/blob/main/wrangle_act.ipynb)

2. [Data Wrangling Report](https://github.com/Waga43/EduTechTainMent_Udacity_Data_Analyst_ND_Project_Wrangle_and_Analyze_WeRateDogs_Twitter_Data/blob/main/wrangle_report.html)

3. [Act Report](https://github.com/Waga43/EduTechTainMent_Udacity_Data_Analyst_ND_Project_Wrangle_and_Analyze_WeRateDogs_Twitter_Data/blob/main/act_report.pdf)
