![Swire Project Banner](./misc/swire-banner.png)

# Swire Delivery Standardization | University of Utah MSBA

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

All analyses, insights, and recommendations presented in this repository were developed using the resources provided by Swire, including sanitized datasets, data dictionaries, related documentation, and follow-up Q&A. All findings and proposals are grounded in the data and materials supplied, and reflect interpretations derived solely from those resources.

The main challenge we encountered was the ambiguity of the project. During the project introduction, there were some complicting priorities between identifying high potential customers and delivery cost savings. Another challenge we faced was the limited data we had. As previously mentioned, one priority was delivery cost savings, however, we did not receive delivery cost data until very late, so we weren't able to focus on that as much. Additionally, having only 2 years of data made it challenging to accurately evaluate things like the relationship of customer tenure to the value the bring to Swire. Similarly, we were also not given any revenue data to be able to quantify what impact our segmentation strategy had on revenue. While we were able to identify the volume retained in each distibution model, it would have been beneficial to be able to translate that into revenue to further support our argument that, while our proposal didn't save on transporation costs, we retained more revenue, and *potentially* observed improved profit margins.

## My Contribution

For this project, I created a data cleaning script, performed exploratory data analysis which focused on identifiying patterns in catagorical variables, year-over-year volume growth by customer, and analyzing the relationship between the two. For the modeling portion of this project, I focused on creating a forecast model to forecast customer level ordered volume. Going into the modeling portion, I recognized the immediate challenges with creating a forecast model as we only had 2 years of data, which is typically not sufficient enough. However, I wanted to proceed with this approach as I thought it would provide value by identifying the features that improve the model and to gain insights on what else would be needed to develop a more robust forecast model. The goal of this was to be able to identify which types of customers observe high growth from the beginning of the relationship with Swire in order to forecast potential voulme for new customers, allowing Swire to make decisions earlier on in the relationship regarding distribution strategy. 

## Takeaways

This project was very enjoyable but there were challenges that I faced individially and that my team faced together. Being new to world of data analytics, I still struggle a bit with project ambiguity, and it was very prevalant here. This project was a clear indication that real world business problems have quite a bit of ambiguity and it is the analysts resposibility to work through that. This is something I still need to work on, but I learned a lot about how to handle the ambiguity through the group work my team did and the frequent conversations we had visiting and revisiting the business problem. Additionally, this project gave me a lot more experience working with limited data and improved my feature engineering skills. During my modeling approach, I performed quite a bit of feature engineering for my forecast model, and each approach I took, whether it was needing to include more new features or removing unnecessary features, taught me which areas I need to focus more on and which areas require less attention. This also exposed some time management improvements I can make in the future as I was so focused on creating a very good model and by the time I did, there was limited time to extract more insights to be able to include my model in our final presentation and reccomendation. 
