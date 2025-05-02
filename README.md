# 📊 Global YouTube Statistics Dashboard

## 🌐 Overview

This project analyzes a dataset of global YouTube statistics from 2023, focusing on the most subscribed channels. The goal is to provide insights into the top creators, content categories, geographical distribution, and the relationship between YouTube performance and socio-economic indicators.

- 🛠️ **Dashboard:** Google Looker Studio  
- 🐍 **Data Processing:** Python (Google Colab)  
- ☁️ **Storage & Querying:** Google BigQuery

---

## 📁 Data Source

**Dataset:** [Global YouTube Statistics 2023 – Kaggle](https://www.kaggle.com/datasets/nelgiriyewithana/global-youtube-statistics-2023/data)  
📌 Contains subscriber counts, views, uploads, countries, earnings, and socio-economic data.

---

## 🔄 Data Processing

1. 🧹 **Python Transformation (Colab):**
   - Missing values handled
   - Columns renamed
   - Date column constructed from `created_year`, `created_month`, and `created_date`

2. 🗃️ **BigQuery Table:**
   - Processed CSV loaded into BigQuery

3. 🔍 **BigQuery View:**
   - `created_month` (text) converted to numeric for visualization purposes

4. 📈 **Dashboard Creation (Looker Studio):**
   - Multi-page dashboard built using the dataset and transformed views

---

## 🗺️ Dashboard Structure & Insights

### 🔹 Page 1 – Global YouTube Overview

**🧭 Filters:**  
- **Period:** Allows analysis of trends over time.
- **Category:** Enables focusing on specific types of YouTube channels.
- **Country:** Facilitates comparisons of performance across different regions.

**📌 KPIs:**  
- Total Channels  
- Avg Subscribers  
- Avg Views/Video  
- Avg Monthly Earnings  

**📊 Charts an Insights:**
- **Top 10 Channels by Subscribers:**
  - T-Series leads significantly with 245 million subscribers.
  - YouTube Movies and MrBeast compete closely for the second position.
  - The top 10 includes various content types (music, kids, entertainment, media).
  - Four channels focus on children's content.
  - The high number of subscribers for channels indicates a considerable barrier of entry for new channels to achieve this level of popularity and reach.

- **Channels by Category:**  
  - "Entertainment" has the highest number of channels (256).
  - "Music" ranks second with 204 channels, reflecting the vast range of musical content present on YouTube.
  - Categories like "News & Politics," "Science & Technology," and "Sports" have fewer channels.
  - Smaller categories might represent opportunities for creators in less saturated markets.
  - The distribution suggests the types of content most produced, though not necessarily the most viewed.
 
- **Views by Category:**  
  - "Music" leads with 3.1 trillion views.
  - "Comedy", "Film & Animation" and "Shows" demonstrate a constant consumption of audiovisual entertainment content.
  - When comparing this graph with the "Channels by Category" graph, we can see that categories with many channels do not always correspond to the categories with the most views.
  - Categories with the highest volume of views often represent the biggest monetization opportunities for content creators due to the greater potential for ad reach.

- **Channels by Country:**  
  - The USA shows the largest concentration of channels. This suggests a strong content creation culture and a large creator base in this region.
  - India and other parts of Asia have a substantial number of channels.
  - Channels are more dispersed across Europe.
  - The map highlights a clear disparity in the number of channels between different regions of the world, possibly influenced by factors such as internet access, technological infrastructure, and digital culture.
  - Less represented regions may offer significant growth potential.

---

### 🔹 Page 2 – Performance by Region and Social Indicators

**🧭 Filters:**  
- **Period:** Allows analysis of trends over time.
- **Category:** Enables focusing on specific types of YouTube channels.
- **Country:** Facilitates comparisons of performance across different regions.

**📊 Charts an Insights:**
- **Revenue vs. Population:**  
  - The relationship between population and estimated annual revenue is not strictly linear. Countries with similar populations may have very different estimated annual revenues, suggesting other factors at play, such as audience engagement, monetization rates, and purchasing power.

- **Revenue vs. Urbanization:**  
  - The scatter of points on the graph suggests that the relationship between urbanization and estimated average monthly income is not a strict rule, with other factors such as the purchasing power of the urban population, the quality of content, and monetization strategies playing important roles.

- **Subscribers vs. Unemployment Rate:**  
  - The scatter of points on the graph suggests a weak or nonexistent direct linear correlation between a country’s unemployment rate and the total number of subscribers to its channels. Countries with similar unemployment rates may have very different subscriber numbers, and vice versa.

- **Monthly Subscriber Growth by Country:**  
  - This graph may indicate emerging trends in YouTube's popularity across different regions, with some countries experiencing faster growth than others.
  - The United States shows the highest monthly growth. This indicates a strong growth and popularity dynamic for new and existing channels in the US.
  - Indonesia also has robust monthly subscriber growth, suggesting a growing YouTube market and an audience that is engaged with new content.

---

### 🔹 Page 3 – Advanced Analytics & Insights

**🧭 Filters:**  
- **Period:** Allows analysis of trends over time.
- **Category:** Enables focusing on specific types of YouTube channels.
- **Country:** Facilitates comparisons of performance across different regions.

**📊 Charts an Insights:**
- **Subscriber Growth vs. Earnings:**  
  - Most channels cluster in the bottom left of the chart, indicating more modest monthly subscriber growth and lower average monthly revenue. This represents the vast majority of creators in the sample.
  - The scatter of points suggests that there is not a strong, direct linear correlation between monthly subscriber growth and average monthly revenue for all channels. High subscriber growth does not always immediately translate into high revenue, and vice versa.

- **Highest Views per Video:**  
  - The presence of Bad Bunny (music) and channels such as LUCCAS NETO (children's entertainment) and Badabun (entertainment/news) suggests that these niches tend to generate a high number of views per video.
  - A high average number of views per video suggests a loyal, engaged audience that returns to watch new content.

- **Earnings Evolution by Category (Bar Chart):**  
  - The “Entertainment” category consistently posts the highest estimated earnings across all months of the year, with notable spikes in January and July. This reinforces the idea that entertainment content is a major revenue generator on the platform.
  - Some categories show seasonal variations in earnings. For example, “Music” peaks in March, while “Entertainment” peaks in January and July. This could be related to specific events, content releases, or audience viewing patterns.

---

## ✅ Conclusion

This dashboard provides a global view of the 2023 YouTube ecosystem, revealing:

- Key performers  
- Strategic insights by region  
- Trends between content and social factors  

Useful for:
- Content Creators  
- Marketers  
- Platform Analysts  

➡️ There’s still room to uncover deeper insights through further exploration of this rich dataset.

---

## 📚 Citation

If you use this project or the data for academic or analytical purposes, please cite the original dataset:

> Nidula Elgiriyewithana. (2023). *Global YouTube Statistics 2023* [Data set]. Kaggle. https://doi.org/10.34740/KAGGLE/DSV/6211042
