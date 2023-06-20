The data directory contains the dataset used in this research project. The dataset comprises tweets, government publications, and news reports related to this research project.

### Dataset Description

The dataset consists of the following files:

1. **online_citizen.pkl**: This pickle file contains a collection of tweets gathered from various users from India, Bangladesh and United States. This is a redacted version, as per the Ethics Approval from the UNSW Committee. 
2. **traditional_media.pkl**: The pickle file contains a compilation of news reports obtained from India, Bangladesh and United States. For India, it contains news reports from Times of India and Hindustan Times. For Bangladesh, it is Daily Star and Dhaka Tribune. For the US, it is NYT and WP. 
3. **government.pkl**: The pickle file contains government publications from India, Bangladesh and United States.


### Data Format

- **online_citizen.pkl**: The file follows a tabular structure with the following columns:
  - Publication_Date: date the tweet was tweeted. In %d-%b-%y format
  - Origin: [contains the list of redacted usernames of Twitter users
  - Origin_Body: contains the raw tweets
  - Origin_Geocode: {'India': 1, 'USA': 2, 'Bangladesh': 3}
  - Source_Type: contains the type of source that was used in the tweet, as per the descriptions listed in the dissertation. (i.e. government, news agency, social media..)
  - Source_Nationality: contains the nationality of the source.
  - Phase : contains the conflict phase when the tweet was tweeted, represented by the respective values 1, 2, and 3.


- **news_reports.pkl**: The file follows a tabular structure with the following columns:
  - Publication_Date: date the news report was published. In %d-%b-%y format
  - Origin: {Times of India' : 1, 'Hindustan Times':2 ,'Daily Star':3, 'Dhaka Tribune':4,'New York Times':5, 'Washington Post': 6}
  - Origin_Body: contains the raw news report
  - Origin_Geocode: {'India': 1, 'USA': 2, 'Bangladesh': 3}
  - Source_Type: contains the type of source that was used in the report, as per the descriptions listed in the dissertation. (i.e. government, news agency, social media..)
  - Source_Nationality: contains the nationality of the source
  - Headline: contains the headline of the news report
  - Phase: contains the conflict phase when the report was published, represented by the respective values 1, 2, and 3 


- **government.pkl**: The file follows a tabular structure with the following columns:
  - Publication_Date: date the publication was published. In %d-%b-%y format
  - Origin: {'Government': 7}
  - Origin_Body: contains the raw government publications.
  - Origin_Geocode: {'India': 1, 'USA': 2, 'Bangladesh': 3}
  - Headline: contains the headline of the news report
  - Phase : contains the conflict phase when the government publication was published, represented by the respective values 1, 2, and 3.
