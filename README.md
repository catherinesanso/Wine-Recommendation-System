Catherine Sanso <br>

# **Speech Emotion Recognition**

## Table of Contents:

1. [Background](#section-title)
1. [Problem Statement](#section-title) 
1. [Research Approach](#section-title)
1. [Data Dictionary](#section-title)
1. [Discussion & Recommendations](#section-title)
1. [Software Required](#section-title) 
1. [Sources](#section-title)
1. [Licensing](#section-title)

# [Background](#section-title)

Recommendation systems, often referred to as recommender systems or recommendation engines, are a cornerstone of modern digital experiences. They are the algorithms behind personalized suggestions that we encounter in our daily online interactions, whether it's movie recommendations on Netflix, product suggestions on Amazon, or playlist recommendations on Spotify. These systems are designed to analyze and understand user preferences and behavior, enabling platforms to provide tailored content, products, or services.

There are several types of recommender systems, including popularity models, content-based filtering, and collaborative filtering, each with its unique approach to delivering personalized recommendations.
- Popularity models rely on the wisdom of the crowd, recommending popular items to users.
- Content-based filtering leverages the attributes of items and a user's past behavior to make suggestions.
- Collaborative filtering examines user behavior and preferences to identify similar users and recommend items they liked.

Recommender systems have revolutionized industries like e-commerce, content streaming, and online advertising by boosting user engagement, increasing customer satisfaction, and driving revenue growth. These systems not only enhance user experiences by reducing information overload but also play a vital role in business success by optimizing product discovery, personalization, and customer retention.


# [Problem Statement](#section-title)

I am leading a team of consultants who are tasked with pitching recommendation systems to executives at Wine.com. There is great potential in leveraging the website's vast user and product data to drive revenue and enhance user experiences. The challenge is harnessing this wealth of information effectively. My proposal is to implement three key recommender systems tailored to Wine.com's business:

1. **Popularity Model**: This system will showcase the most popular wines, enticing users with the collective wisdom of fellow wine enthusiasts. By prominently featuring these selections, you'll not only increase sales of popular wines but also improve user engagement.

2. **Content-Based Filtering**: Leveraging the attributes of wines and users' past behavior, this system will offer personalized wine recommendations. It enhances user satisfaction by providing relevant choices, thereby increasing conversion rates and customer loyalty.

3. **Collaborative Filtering**: By analyzing user behavior and preferences, this system identifies like-minded wine enthusiasts and recommends wines based on their shared interests. This fosters a sense of community, driving user engagement and fostering repeat business.

Incorporating targeted advertisements within these recommender systems will boost ad relevance and click-through rates, maximizing ad revenue. Furthermore, these systems will gather valuable user insights, allowing you to refine your product offerings and marketing strategies.

Ultimately, our recommendation engines will significantly enhance the user experience, drive sales, and increase user retention. They provide the means to deliver tailored advertisements, which, in turn, will maximize ad revenue. With these systems in place, Wine.com will not only satisfy existing customers but also attract new ones, fostering long-term growth and profitability.


# [Research Approach](#section-title)

- The dataset is scraped from __[Wine.com](https://www.wine.com/list/wine/red-wine/7155-124?sortBy=mostInteresting)__ and the user_id numbers and individual product ratings are hypothetically configured, as that data is proprietary to Wine.com and could not be accessed for the purposes of this research. 

# [Data Dictionary](#section-title)

The following terms and abbreviations are used throughout this project and are defined as follows:

| Item | Description
| --- | --- 
| **product_id** | *Product ID per wine sold*
| **wine_type** | *Type of Wine*
| **wine_name** | *Name of Wine*
| **wine_origin** | *Wine Origin (region or city, country)*
| **rating_avg** | *The average rating per product_id*
| **ratin_num** | *The number of ratings provided for each product_id*
| **price_current** | *The current price displayed on Wine.com's website*
| **price_prediscount** | *The prediscounted price displayed on Wine.com's website*
| **discount_nom** | *The nominal discount value, in USD ($)*
| **savings_percent** | *The percent discount offered from the prediscounted and current prices*
| **user_id** | *User ID*
| **event_type** | *Type of interaction user may have with Wine.com, including view, like, rate, comment, follow, bookmark* 
| **event_strength** | *Strenght of event type, from 1 to 4.5 (discretionary)* 
| **user_weighted_sum** | *Weighted sum of all event_types and event_strengths per user*

# [Discussion & Recommendations](#section-title)

In choosing the ideal recommendation model for Wine.com, it's crucial to consider the strengths and weaknesses of each approach and seek ways to enhance their performance.

**Popularity Model**: The Popularity Model, highlighting the most popular wines, provides a simple yet effective way to engage users. To make it even better, we should continuously update the popularity rankings based on real-time user interactions. Additionally, analyzing user reviews and ratings can provide more nuanced insights into wine preferences.

**Content-Based Filtering**: Content-Based Filtering is excellent for personalization, but it relies heavily on product attributes. To improve this system, enrich the product data with additional attributes like tasting notes, wine awards, or sommelier recommendations. Gathering more detailed user data, such as wine tasting history or preferences, will also boost accuracy.

**Collaborative Filtering**: Collaborative Filtering is powerful for identifying user affinities, but it can suffer from the "cold start" problem with new users or products. To mitigate this, encourage users to rate wines upon sign-up and prompt new users with initial recommendations based on their stated preferences.

Another option to consider would be a hybrid recommendation model:

**Hybrid Recommendation Model**: A Hybrid Recommendation Model, combining the strengths of multiple approaches, can offer the best of all worlds. It can intelligently switch between models based on user behavior and the availability of data. For instance, use collaborative filtering for active users and content-based filtering for newcomers.

To enhance all these models, invest in data collection mechanisms, employ sentiment analysis on user reviews, and employ natural language processing to better understand user preferences. By embracing a hybrid model and continually refining your data-driven strategies, Wine.com can optimize user experiences and drive increased revenue.

# [Software Required](#section-title)
The software required for this project are listed on the first line of code within each notebook and include: Pandas, Beautiful Soup, Requests, Numpy, MatplotLib, Random, SKLearn, and Surprise.

# [Sources](#section-title)

General:
- [Wine.com](https://www.wine.com/list/wine/red-wine/7155-124?sortBy=mostInteresting)
- [Towards Data Science: Recommender Systems](https://towardsdatascience.com/introduction-to-recommender-systems-6c66cf15ada)
- General Assembly Notes & Lectures
- Stack Overflow & ChatGPT

# [Licensing](#section-title)
This project is licensed under the MIT license.
