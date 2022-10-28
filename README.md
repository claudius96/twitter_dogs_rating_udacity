### Twitter dog rating dataset

## Dataset overview
This part of the data was taken from WeRateDogs twitter account through twitter API

## Wrangle Report
I had three datasets to work with the first twitter_archive dataset, twitter API data and image predictions tsv file. I first gathered all these data twitter_archive dataset, image_predictions and twitter API datasets I used requests method to download all them as files in my working directory.

From the gathering process I assessed these datasets. I was able to find couple number of problems in the dataset which include misrepresented data types, rating denominators below and above 10 whilst they're supposed to 10, I noticed tidness issues where variable is to form a column but 1 variable had formed many columns.

from the assessment of the data I then cleaned the data,I placed doggo, floofer, pupper and puppo into a single column  which i named dog stages. I changed timestamp datatype from object to datetime. I made sure that rating denominators where equal to 10 for all the rows in the dataset.

### Insights:
1. I was able to find that there a correlation between retweet_counts and favorite_counts

2.  I noted that dog_stage  does not matter in giving higher or lower ratings

### Conclusions
- we can note that there is a positive correlation between favorite_count and retweet_count. With all other factors that are likely to affect retweet count set aside, we can safely say that a picture of a dog liked as favorite is most likely to be retweeted.

- Apart from other dogs that had the most favorite counts but didn't have names we can see that Jamesy was the dog with a name with the most favorite counts.

- although we can see much outlier rating in pupper dog age, we can safely say there is not much of a relationship between the dog's age and its rating