# Amazon Product Sales Analysis with Power BI

### Project Objective

Amazon is an American Tech Multi-National Company whose business interests include E-commerce, where they buy and store the inventory, and take care of everything from shipping and pricing to customer service and returns. 
So, get a dataset about Amazon sales product reviews, transform and analyze it with insights on product category reviews and rating distributions, and give recommendations for effective data-driven decisions.

- Note: This Company (Our Client), wanted to start an E-commerce business like Amazon, so, they wanted analysis on such type of business as direction.

### Data Source

The Dataset was in CSV file format that was downloaded from the public website. I can only provide a related link to this dataset and not the same. 
You can download a sample here – [kaggle.com]( https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset)

### Tools Used

Power BI — Data Cleaning, Transformation, Analysis, and Creating Reports.

### Data Cleaning and Preparation

The dataset has 1,465 rows and 16 columns featuring product_id, product_name, category, discounted_price, actual_price, discount_percentage, rating_count, about_product, etc. This dataset has over 1,000 Amazon Product Ratings and Reviews.

#### Cleaning Processes
  
 - Price Format: The "discounted_price" and "actual_price" columns had formatting issues. The prices are represented in a format that includes a currency symbol (â‚¹) and commas. It was helpful to transform these columns into a numerical format (e.g., I removed the currency symbol and commas) for quantitative analysis.
 - Rating Count: The "rating_count" column needed transformation to remove commas and convert it into a numerical format for analysis.
 - Image and Product Links: The "img_link" and "product_link" columns contain URLs to images and product pages. These columns were not needed for the analysis so they were removed from the table or dataset.
 - Review Titles and Content: The "review_title" and "review_content" columns also benefited from text preprocessing, such as handling special characters.
Category.
 - The "category" column had a hierarchical structure using pipe (|) as a separator. Because I needed the column for analysis, I had to split this column into multiple categorical columns for better categorization.
 - Conditional Column: I created a conditional column for the rating with the column as rating_1 to represent the categories of customer rating as 5 = Very Good, 4.0-4.9 = Good, 3.0-3.9 = Average, 2.0-2.9 = Fair, 1.0-1.9 = Poor.

### Exploratory Data Analysis (EDA)

The following key Performance Indicators (KPIs) and insights were generated:
-	Average Discount Percentage = 0.55
-	Sum of Discounted Price = 4M
-	Average Rating = 4.10
-	Total Sales = 4M
-	Total Number of Reviews = 1,465
-	Sum of Actual Price = 7M
-	Top Categories by Sales
-	Sum of Discount Percentage by Product Name
-	Distribution of Ratings
-	Average Rating by Categories
-	Total Sales by Product 

### Data Analysis

#### Key Performance Indicators (KPIs)
~~~
-	AVG Discount % = AVERAGE(amazon_1[discount_percentage])
-	Sum of Discounted Price = SUM(amazon_1[discounted_price])
-	Average Rating = AVERAGE(amazon_1[rating])
-	Total Sales = SUM(amazon_1[discounted_price])
-	Number of Reviews = COUNTROWS(amazon_1)
-	Sum of Actual Price = SUM(amazon_1[actual_price])
~~~

#### Analytical Insights

-	Top Categories by Sales: Explored the distribution of sales across different product categories. This gave insights into which product categories contribute the most to the overall sales.
-	Sum of Discount Percentage by Product Name: Compared the distribution of discount percentages which provided insights into the level of discount across the products.
-	Distribution of Ratings: Also explored the impact of the distribution of customers’ ratings. This helped to show the sum of customer reviews with the highest rating of “Very Good”, “Good”, “Average”, “Fair”, and “Poor’. 
-	Average Rating by Categories: This shows the product category with the highest percentage of rating.
-	Total Sales by Product: This insight reviews the bestselling product.

#### Visualization

Generated the following visual analyses using Power BI.

#### Top Categories by Sales:

![1](https://github.com/Solution92/Amazon-Product-Sales-Analysis-with-Power-BI/assets/144762124/068b4df7-5b8a-4ae1-b81d-79bf59f45bb3)

#### Sum of Discount Percentage by Product Name:

![2](https://github.com/Solution92/Amazon-Product-Sales-Analysis-with-Power-BI/assets/144762124/e9aa6362-4171-408c-9493-371030881515)

#### Distribution of Ratings:

![3](https://github.com/Solution92/Amazon-Product-Sales-Analysis-with-Power-BI/assets/144762124/92cc1350-2bb1-4122-86ee-1255b9c2a89a)

#### Average Rating by Categories:

![4](https://github.com/Solution92/Amazon-Product-Sales-Analysis-with-Power-BI/assets/144762124/f0eddb18-0f4d-474d-b333-37bb85d24174)

#### Total Sales by Product:

![5](https://github.com/Solution92/Amazon-Product-Sales-Analysis-with-Power-BI/assets/144762124/abc5dd78-e5af-49b7-ab99-df6fa741ccd6)

#### The Dashboard

![Screenshot_121](https://github.com/Solution92/Amazon-Product-Sales-Analysis-with-Power-BI/assets/144762124/29055310-eecf-414a-ac03-09577e518af9)


### Result and Findings

Concerning my analysis of Amazon Product Sales with Power BI, here are my findings;

-	In Sum of Discount Percentage by Product Name, At 7.20, Sounce Fast Phone Charging Cable & Data Sync USB Cable Compatible for iPhone 13, 12,11, X, 8, 7, 6, 5, iPad Air, Pro, Mini & iOS Devices, had the highest Sum of discount percentage and was Infinity higher than Samsung Original Type C to C Cable - 3.28 Feet (1 Meter), White, which had the lowest Sum of discount percentage at 0.  
-	Sounce Fast Phone Charging Cable & Data Sync USB Cable Compatible for iPhone 13, 12,11, X, 8, 7, 6, 5, iPad Air, Pro, Mini & iOS Devices, had the highest Sum of discount percentage at 7.20, followed by PTron Solero T241 2.4A Type-C Data & Charging USB Cable, Made in India, 480Mbps Data Sync, Durable 1-Meter Long USB Cable for Type-C USB Devices for Charging Adapter (Black) and Lapster 1.5 mtr USB 2.0 Type A Male to USB A Male Cable for computer and laptop. Samsung Original Type C to C Cable - 3.28 Feet (1 Meter), White had the lowest Sum of discount percentage at 0.  
-	Sounce Fast Phone Charging Cable & Data Sync USB Cable Compatible for iPhone 13, 12,11, X, 8, 7, 6, 5, iPad Air, Pro, Mini & iOS Devices accounted for 1.30% of Sum of discount percentage.  Across all 126 product name, the Sum of discount percentage ranged from 0 to 7.20.  
-	Also, in the Distribution of Ratings, At 840, “Good”, had the highest Number of Reviews and was 425.00% higher than “Average”, which had the lowest Number of Reviews at 160.  
-	“Good”, had the highest Number of Reviews at 840, followed by at 465 and “Average”, at 160.  
-	“Good”, accounted for 57.34% of Number of Reviews.   
-	Had 465 Number of Reviews, “Good”, had 840, and “Average”, had 160.  
-	Meanwhile, in Total Sales by Product, Redmi 126 cm (50 inches) 4K Ultra HD Android Smart LED TV X50 | L50M6-RA (Black) and OnePlus 126 cm (50 inches) Y Series 4K Ultra HD Smart Android LED TV 50Y1S Pro (Black) tied for highest Total Sales at 263992, followed by Samsung 108 cm (43 inches) Crystal 4K Neo Series Ultra HD Smart LED TV UA43AUE65AKXXL (Black). 
-	Across all 126 product name, Total Sales ranged from 472 to 263,992.  


### Recommendation

Based on the analysis of Amazon Product Sales dataset with Power BI, here are some recommendations for the products:
- Discount Strategies: Consider reviewing the discount strategy for the product with the highest Sum of Discount Percentage, "Sounce Fast Phone Charging Cable & Data Sync USB Cable Compatible for iPhone 13, 12,11, X, 8, 7, 6, 5, iPad Air, Pro, Mini & iOS Devices" with a Sum of discount percentage at 7.20. Assess whether such a high discount is driving sales effectively or if there are alternative strategies to increase sales without significant discounts.
- Product Focus: Given that "Sounce Fast Phone Charging Cable..." accounts for a significant portion (1.30%) of the total Sum of Discount Percentage, evaluate its overall performance in terms of sales and profitability. If it's a high-performing product, consider optimizing its marketing and distribution channels.
- Review Ratings Impact: Products with a "Good" rating category seem to have the highest number of reviews. Consider investigating the factors contributing to positive reviews and leverage this information in marketing strategies. It might also be beneficial to address any concerns or issues raised by users with lower ratings.
- Product Diversification: Explore opportunities to diversify the product portfolio. While TVs like "Redmi 126 cm (50 inches) 4K Ultra HD Android Smart LED TV X50" and "OnePlus 126 cm (50 inches) Y Series 4K Ultra HD Smart Android LED TV 50Y1S Pro" are top performers, expanding into other categories or introducing new products could enhance the overall product offering.
Marketing and Visibility: Products with lower reviews and ratings might benefit from enhanced marketing efforts to increase visibility and improve customer perception. Implement targeted marketing campaigns, promotions, or product improvements to boost sales and reviews.
- Competitive Analysis: Conduct a competitive analysis, especially for products with lower sales. Understand the market landscape, pricing strategies of competitors, and customer preferences. This analysis can provide insights into areas where your products can stand out or be more competitive.


### Limitation 

Here are a few potential limitations that should be considered:
- Lack of Key Metrics: The dataset seems to be missing some key metrics that could provide deeper insights. For example, it lacks information on actual sales, profit margins, or revenue. Without these metrics, it may be challenging to assess the financial performance of each product accurately.
- Limited Time Dimension: The absence of a timestamp or date field limits the ability to analyze sales performance over time. Insights into seasonality, trends, or the impact of time-related factors on sales are not possible without this information.
- Limited Product Information: While the dataset includes information on product names, discounted prices, and actual prices, it lacks detailed product specifications, features, or attributes. This limitation may restrict the depth of analysis related to specific product characteristics that influence sales.
- Single Platform Data: If the dataset represents sales data from a single platform (e.g., Amazon), it might not capture a comprehensive view of the market. Understanding sales performance across multiple platforms or channels could provide a more holistic perspective.


### Reference

For product sales from E-commerce stores and related, you may refer to kaggle.com


#data #loan #decision #application #analysis #approval #finance #communication #teamwork #powerbi



