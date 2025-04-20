![Swire Project Banner](./misc/swire-banner.png)

# Swire Delivery Standardization | University of Utah MSBA | Georgia Christodoulou

Repository featuring individual work for data prep, analysis, modeling, and group proposals for segmenting the delivery business models of Swire Coca-Cola.

## Project Summary

### Description

Swire Coca-Cola (SCCU) operates under two distribution models: “Red Truck” for high-volume customers serviced directly by Swire, and “White Truck” or “Alternate Route to Market” for smaller customers served by third-party distributors. Swire’s current segmenting strategy has led to misallocation of resources, inflated expenses, and missed opportunities from clients with high-growth potential. Swire seeks to improve alignment between customers and the appropriate distribution model by analyzing customer characteristics and ordering behaviors to support long-term success.

### Solution and Business Value

It's recommended that Swire Coca-Cola adopt an alternate strategy to the incumbent, 400-gallon threshold to segment customers between RED TRUCK and WHITE TRUCK programs, specifically leveraging customer characteristic combinations and market indicators (below).

<p align="center">
  <img src="misc/segmentation-strategy-1.png" alt="Segmentation Strategy 1" width="45%" />
  <img src="misc/segmentation-strategy-2.png" alt="Segmentation Strategy 2" width="45%" />
</p>

The following insights gleaned from our cleaning, analysis, and modeling work indicate this approach to be superior to a "one size fits all" rule while remaining intuitive and fairly simple:

* Annual volume is a noisy measure for RED TRUCK material as a majority of customers qualifying under the incumbent strategy did so via a high touch, inefficient ordering method
* Customer characteristics do well to predict segmentation independent of the target volume threshold, indicating they should play a key role in the strategy
* Market dynamics are an important component and summarizing the performance of the closest neighboring customers does well to approximate local market conditions

Adoption of this strategy strikes a good balance between capturing future opportunity and preserving an efficient red truck program. 

<p align="center">
  <img src="misc/segmentation-strategy-3.png" alt="Segmentation Strategy 3" width="45%" />
</p>

We found this strategy to retain 56% more volume in 2025 than the incumbent strategy, while achieving 86% of the incumbent strategy's RED TRUCK program efficient of 2025 volume per $100 of delivery costs.

We recommend Swire Coca-Cola validate the results of this project with original data sets and implement components thereof to improve the segmentation strategy for delivery model programs. 

Thank you,

Adam, Georgia, Tyler, Zac

## Challenges

All analyses, insights, and recommendations were based on sanitized datasets and supporting documentation provided by Swire. One major challenge was the ambiguity of the project goals. Early on, there were competing priorities between identifying high-potential customers and reducing delivery costs.

We also faced data limitations. Delivery cost data, which was critical for assessing efficiency, was provided very late in the project. Additionally, we only had access to two years of customer-level data, which limited our ability to explore longer-term patterns, such as tenure-based value or lifecycle growth.

Another gap was the absence of revenue data, which made it difficult to directly assess the financial impact of our segmentation strategies. While we were able to measure volume retained across strategies, we could not quantify whether our recommendations improved revenue or profit margins. Translating volume gains into revenue impact would have strengthened our case.

## My Contribution

For this project, I created a data cleaning script and performed exploratory analysis, with a focus on uncovering relationships between categorical variables and year-over-year volume growth by customer. I also developed the forecast model to estimate customer-level volume, which aimed to help identify traits linked to early growth. While building the model, I recognized challenges due to the short, 2-year timeframe. Despite this, I pursued the modeling approach to extract meaningful insights about growth predictors and identify areas where Swire could improve early decision-making for new customers. The goal of the model was to support earlier distribution decisions by highlighting high-growth potential customers before a long history develops. This contributed to our recommendation to shift away from a static volume threshold and toward a more predictive, customer-informed strategy.

## Takeaways

This project was both rewarding and challenging. One of my biggest takeaways was learning how to navigate project ambiguity. Real-world business problems rarely come with clear boundaries, and I had to learn how to frame and reframe the problem collaboratively with my team.

I also gained valuable experience working with limited and delayed data, which required flexibility in both analysis and modeling. During the modeling phase, I experimented with various feature engineering techniques to improve forecast accuracy, learning which types of features added value and which didn’t.

Finally, I learned the importance of time management. I was highly focused on building a strong model, but with more time, I could have better integrated those insights into our final presentation and recommendations. This project helped me grow both technically and professionally, especially in areas like working through ambiguity, prioritizing model interpretability, and balancing analysis with business communication.

