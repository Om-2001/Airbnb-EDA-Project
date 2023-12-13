# Airbnb Exploratory Data Analysis (EDA) Project by Om Kalbhor

## Introduction

This EDA project aims to analyze the Airbnb dataset, uncovering valuable insights into pricing patterns, room types, host behavior, and geographical trends. The primary objectives include understanding user preferences, identifying influential factors on pricing, and providing actionable insights for both hosts and guests.

## Notebook Breakdown

1. **Importing Libraries:**
   - Utilized essential data science libraries such as NumPy, Pandas, Matplotlib, Seaborn, and Google Colab for efficient analysis.

2. **Loading Dataset:**
   - Loaded the Airbnb dataset from a specified file path using Pandas.
   
3. **Data Wrangling:**
   - Renamed columns for clarity: `neighbourhood_group` to `location` and `neighbourhood` to `area`.
   - Dropped unnecessary columns (`latitude`, `longitude`, `last_review`, `reviews_per_month`).
   - Handled missing values in `name` and `host_name` columns by dropping relevant records.
   - Removed rows with zero prices.
   - Converted categorical columns (`room_type`, `location`, `area`) to the 'category' data type for better analysis.
   
4. **Dataset Summary:**

    - Dataset Columns:
      - **id**: Unique identifier for each Airbnb listing.
      - **name**: The name or title of the listing.
      - **host_id**: Unique identifier for the host of the Airbnb listing.
      - **host_name**: The name of the host.
      - **location**: The broader geographical area or group of neighborhoods that the listing is located in.
      - **area**: The specific neighborhood where the listing is situated.
      - **latitude**: The latitude coordinate of the listing's location.
      - **longitude**: The longitude coordinate of the listing's location.
      - **room_type**: The type of room or accommodation offered (e.g., entire home/apartment, private room, shared room).
      - **price**: The price per night for the listing.
      - **minimum_nights**: The minimum number of nights a guest is required to stay.
      - **number_of_reviews**: The total number of reviews the listing has received.
      - **last_review**: The date of the last review received for the listing.
      - **reviews_per_month**: The average number of reviews the listing receives per month.
      - **calculated_host_listings_count**: The count of listings managed by the host.
      - **availability_365**: The number of days the listing is available for booking within a year (365 days).

   - Detailed overview of the dataset:
      - Unique identifiers (`id`, `host_id`).
      - Listing details (`name`, `room_type`, `price`, `minimum_nights`).
      - Host information (`host_name`, `calculated_host_listings_count`).
      - Geographical information (`location`, `area`).
      - Review-related information (`number_of_reviews`, `last_review`, `reviews_per_month`).
      - Availability metrics (`availability_365`).

5. **EDA (Exploratory Data Analysis):**
   - Addressed key questions through visualizations and statistical analyses.
   - Explored room type distribution across locations.
   - Analyzed average prices for each room type.
   - Identified preferred areas for guests based on the number of reviews.
   - Explored host preferences for business locations.
   - Examined average prices by area.
   - Investigated the relationship between reviews and prices.
   - Explored the relationship between availability and prices.
   - Analyzed minimum night requirements across neighborhood groups.
   - Identified the top 10 hosts based on the number of listings.
   - Explored the total number of nights spent per room type.
   - Visualized max and min prices for each location and room type.

## Key Insights

- Shared rooms are the least preferred room type, and private rooms are generally favored over entire homes/apartments.
- Manhattan is the preferred location for hosts conducting business.
- Prices follow the expected trend: entire apartment > private room > shared room.
- No significant correlation between the number of reviews, availability, and prices.
- Manhattan has the highest average minimum night requirements.
- Identified the top 10 hosts based on the number of listings.

## Future Scope

- **Sentiment Analysis:** Incorporate sentiment analysis on reviews to understand the quality of listings.
- **Time Series Analysis:** Explore trends in pricing and availability over time.
- **Machine Learning Models:** Develop predictive models for pricing based on various features.
- **Dynamic Mapping:** Utilize geographical coordinates for interactive maps to visualize trends.

## GitHub README Documentation

- Provide a detailed introduction to the project's significance and objectives.
- Summarize the notebook breakdown for easy navigation.
- Include explanations for dataset columns, data wrangling steps, and EDA insights.
- Highlight key findings and actionable insights.
- Suggest potential future directions for analysis and improvement.
