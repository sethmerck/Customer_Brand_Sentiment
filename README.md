# Customer_Brand_Sentiment

Sentiment analysis of comments on e-commerce company website. Discover which products and brands ranked poorly in order to inform buying decisions.

## How It's Made:

**Tech used:** Python libraries - BeautifulSoup, Pandas, Matplotlib, scikit-learn

Scraped comments from product listings and aggregated comments by brand. Information stored in a Python dictionary following the form "{Brand: {Product: [Comments]}}". Then used scikit-learn to perform sentiment analysis on comments. 

Each brand was given a score between 0 and 1 (0 being completely negative and 1 being completely positive) based on amount of positive and negative comments. For example if a brand had 5 positive comments and 5 negative comments, the brand's score would be 0.5 as half of its comments were positive. Scores and brands then placed in pandas dataframe where they could be easily read into a bar chart using matplotlib library of python.

Brand names in figure are altered to preserve anonymity.

-- Only the bottom 5 (0-4) and top 5 (5-9) scoring brands are shown in 'brand_output' chart. --

## Results


## Optimizations
