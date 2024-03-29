# Customer_Brand_Sentiment

Sentiment analysis of comments on product listings of fishing rods scraped from various e-commerce websites. Discovered customer sentiment about products and brands in order to inform buying decisions.

[Link to app](https://sethmerck-comments.streamlit.app/)

## How It's Made:

**Tech used:** Python libraries - BeautifulSoup, Pandas, Matplotlib, Scikit-Learn, Streamlit

Using BeautifulSoup, scraped comments from product listings of fishing rods and aggregated comments by brand. Information stored in a Python dictionary following the form "{Brand: {Product: [Comments]}}". Then used scikit-learn to perform sentiment analysis on comments. 

Each brand was given a score between 0 and 1 (0 being completely negative and 1 being completely positive) based on amount of positive and negative comments. For example if a brand had 5 positive comments and 5 negative comments, the brand's score would be 0.5 as half of its comments were positive. Scores and brands then placed in pandas dataframe where they could be easily read into a bar chart using matplotlib library of python.

Streamlit library then used to generate interactive app visualizing data. Streamlit community cloud service used to feature data visualization on the web for public viewing.

## Results

Most brands had above ~60% positive comments, while a few brands had under 50% positive comments. The brand with the highest percentage of positive comments scored at about 78%, while the lowest ranked brand scored at about 13%.

## Optimizations

Include visualizations for breakdown of comment sentiment within brands to see if certain products of a brand deviate significantly from the overall comment sentiment of that specific brand. This would provide further insight to aid in buying decisions in regards to both brands and the relative popularity of certain products within brands.

Automate data pipeline to routinely update visualization as new comments are placed on sites.
