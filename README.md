# GAP Inc's Big Data Strategy

Using the 2018 HBS case "Predicting Consumer Tastes with Big Data at Gap" by Ayelet Israeli and Jill Avery as a starting point, in this project, we act as third party data consultants trying to help GAP Inc. address the following points :

1. What kind of data can be collected from the web to support the data-driven creative process at Gap? We collect a sample of the data and do appropriate analysis to demonstrate the approach we are suggesting.
2. Does the big data approach work for all three of Gap Inc.’s primary brands: Old Navy, Gap, and Banana Republic? Why or why not?
3. If we are working for the marketing team, how would we leverage web data in balancing the art vs. science in Gap’s marketing strategy?


## Case Background :

GAP faces a problem of declining sales for the past two years. The CEO wants to eliminate
creative directors and eliminate them with a decentralised data driven approach.

We must take into consideration several factors before going about our analysis. 
- First and foremost, there was an industry wise decline in sales and not just in GAP. 
- Millennials were spending less on retail. 
- GAP was offering heavy discounting and had a longer product to market cycle time. 
- GAP coming out with different products was confusing customers and alienating its existing customers. 
- There was heavy competition from other e-commerce brands and other fast fashion brands such as H&M and Zara.

## Data Driven Analysis:
For the data driven analysis, we focused on Reviews, SEO, and Financial Data.

1. **Reviews** (`locations.ipynb`, `gmaps_reviews.ipynb`, `external_reviews.ipynb` & `nlp_analysis.ipynb`)
- Reviews can be bucketed into two - Offline store reviews and online reviews. For
offline reviews we used the store locations of those brands and used browser
automation to complete the scraping of reviews and ratings and time.
- For the online reviews we looked at the external review websites like pissed
consumer and scraped the reviews from there. Many of these didn’t have ratings, so
we did a sentiment analysis using the Azure APIs. As these were mostly negative
reviews, we used the negative confidence score.

2. **Stock Price Comparison** (`finance.ipynb`)
- The chart compares the stock prices of various clothing industry companies from
2010 to 2020.
- Brands compared include GPS (GAP), KSS, M, AEO, URBN, ANF, and DDS.
- GPS experienced a significant peak around 2015, like its 20-year chart.
- Most brands show some parallel movements, especially notable declines around
2015-2016 and again around 2018-2019. This suggests industry-wide trends or
events affecting all these brands.
- AEO and URBN appear to have slightly steadier growth in the latter part of the
decade, while brands like ANF and DDS show more pronounced volatility.
- By 2020, most brands seem to converge in their stock prices, indicating potentially
similar market valuations or industry conditions.
- In summary, while GAP has seen highs and lows over the past two decades, it seems to follow some industry trends, as evidenced by the stock price movements of its competitors. However, individual strategies, brand perceptions, and external factors would contribute to the unique trajectories of each company.

3. **SEO and SERP Analysis** (`keyword_ranking_analysis.ipynb`)
- A higher online presence can potentially lead to increased sales.
- Websites were evaluated based on SEO metrics such as Domain authority, Page authority, Spam score, and Ranking keywords.
SERP Analysis specific to the apparel industry:
- Analysis was done on competitive keywords. The top-ranking brands for each keyword were identified.
- This information was utilized to assess GAP's brand presence and sales.
