# 📊 ChatGPT User Reviews Analysis

## 📝 Project Overview
People have shared a wide range of feedback about the ChatGPT application through ratings and written reviews. This project explores nearly 200,000 user reviews to understand what users love, what frustrates them, and what can be improved. By analyzing sentiment, patterns over time, and common issues, this analysis extracts actionable insights to enhance the user experience.

All data processing, analysis, and visualizations were built using **Microsoft Excel**.

## 🎯 Key Objectives
1. **Sentiment Analysis:** Categorize and identify positive, negative, and neutral user sentiments based on ratings.
2. **Issue Identification:** Detect common problems, bugs, and pain points driving negative reviews.
3. **Time-Series Analysis:** Track how user sentiment evolves over time (month over month).

## 🗂️ Dataset Description
The dataset contains **196,727 records** with the following 4 fields:
* **`Review ID`**: A unique identifier for every review.
* **`Review`**: The written text/comments provided by the user.
* **`Rating`**: Represents the level of satisfaction on a scale of 0 to 5.
* **`Review Date`**: The exact date and timestamp when the review was posted.

## 🛠️ Methodology & Excel Techniques Used
* **Data Transformation:** Used `TEXT()` functions to extract "Year-Month" for chronological tracking.
* **Sentiment Classification:** Utilized nested `IF()` statements (`=IF(Rating>=4, "Positive", IF(Rating=3, "Neutral", "Negative"))`) to map numerical ratings to text sentiments.
* **Text Mining / Issue Tracking:** Leveraged `COUNTIFS()` with wildcard searches (e.g., `*doesn't work*`, `*phone number*`) to calculate the frequency of specific complaints in negative reviews.
* **Data Visualization:** Built dynamic PivotTables and PivotCharts (Bar charts, Line graphs) to visualize distributions and time-series trends.

## 💡 Key Insights & Findings
* **Overwhelmingly Positive Reception:** Approximately **88%** of users leave positive reviews (4 or 5 stars), highlighting high satisfaction with the core AI capabilities.
* **Primary Frustrations (Negative Reviews):** * *App Stability:* The most frequent complaints involve the app crashing or failing to load ("doesn't work", "error occurred").
  * *Server Capacity:* Users often experience downtime or get a "try again later" message during peak hours.
  * *Authentication Friction:* A significant number of negative reviews mention frustration with the mandatory phone number verification process.
* **Growth Trends:** Positive sentiment scales aggressively over time, with massive spikes likely correlating to major OpenAI model updates (like GPT-4o).

## 📂 Repository Contents
* `chatgpt_reviews (2).csv` - The original raw dataset containing the user reviews.
* `ChatGPT_Reviews_Analysis.xlsx` *(Upload your final Excel file and put the name here)* - The completed Excel workbook containing the cleaned data, PivotTables, and the interactive Dashboard.

## 🚀 How to Use
1. Clone the repository or download the `.xlsx` file directly.
2. Open the file in Microsoft Excel.
3. Navigate to the **Dashboard** tab to view the interactive charts.
4. Use the **Slicers** provided on the dashboard to filter the review data by specific months or years.

---
*Created for data analysis portfolio purposes.*
