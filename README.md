# Customer_Brand_Sentiment
Sentiment analysis of comments on e-commerce company website (website lacks rating system). Discover which products and brands ranked poorly in order to inform buying decisions.

## How It's Made:

**Tech used:** Python libraries - BeautifulSoup, Pandas, Matplotlib, scikit-learn

Scraped comments from product listings and aggregated comments by brand. Used scikit-learn to perform sentiment analysis on comments. Each brand was given a score between 0 and 1 (0 being completely negative and 1 being completely positive) based on amount of positive and negative comments. Scores and brands then placed in pandas dataframe where they could be easily read into a bar chart using matplotlib library of python.

Brand names in figure are altered to preserve anonymity.

Only the bottom 5 (0-4) and top 5 (5-9) scoring brands are shown in 'brand_output' chart.
