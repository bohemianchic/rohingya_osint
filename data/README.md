The data directory contains the dataset used in this research project. The dataset comprises tweets, government reports, and news reports related to this research project.

### Dataset Description

The dataset consists of the following files:

1. **online_citizen.pkl**: This pkl file contains a collection of tweets gathered from various users from India and Bangladesh. This is a redacted version to not include the tweet content. 
2. **reports.pkl**: The pkl file contains a compilation of reports obtained from India and Bangladesh
3. **government.pkl**: The pickle file contains government publications from India and Bangladesh


### Data Format

- **online_citizen.pkl**: The file follows a tabular structure with the following columns:
  - Publication_Date: date the tweet was tweeted. In %d-%b-%y format
  - Origin: [contains the list of redacted usernames of users
  - Origin_Body: contains the raw tweets
  - Origin_Geocode: {'India': 1, 'Bangladesh': 2}
  - Source_Type: contains the type of source that was used in the tweet, as per the descriptions listed in the dissertation. (i.e. government, news agency, social media..)
  - Source_Nationality: contains the nationality of the source.
  - Phase : contains the conflict phase when the social media post was posted, represented by the respective values 1, 2, and 3.


- **reports.pkl**: The file follows a tabular structure with the following columns:
  - Publication_Date: date the news report was published. In %d-%b-%y format
  - Origin: {Times of India' : 1, 'Hindustan Times':2 ,'Daily Star':3, 'Dhaka Tribune':4,'New York Times':5, 'Washington Post': 6}
  - Origin_Body: contains the raw news report
  - Origin_Geocode: {'India': 1, 'Bangladesh': 2}
  - Source_Type: contains the type of source that was used in the report (i.e. government, news agency, social media..)
  - Source_Nationality: contains the nationality of the source
  - Headline: contains the headline of the news report
  - Phase: contains the conflict phase when the report was published, represented by the respective values 1, 2, and 3 


- **government.pkl**: The file follows a tabular structure with the following columns:
  - Publication_Date: date the publication was published. In %d-%b-%y format
  - Origin: {'Government': 7}
  - Origin_Body: contains the raw government publications.
  - Origin_Geocode: {'India': 1, 'Bangladesh': 2}
  - Headline: contains the headline of the news report
  - Phase : contains the conflict phase when the government publication was published, represented by the respective values 1, 2, and 3.
