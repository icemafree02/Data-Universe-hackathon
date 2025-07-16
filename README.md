## Data Universe Hackathon 2024
#  Theme: Climate Change

**Project submitted to the Data Universe Final Hackathon 2024**  

This project explores the relationship between **PM2.5 levels**, **weather conditions**, and **tourism-related economic loss** across Thailand between **2020 and 2023**.

---

## 📊 Objective

To understand how air pollution (specifically PM2.5) impacts tourism revenue in Thailand and what weather factors contribute to fluctuations in pollution levels.

---

## 📁 Datasets & Sources

| Dataset Title | Attributes | Timeframe | Source |
|---------------|------------|-----------|--------|
| **Historical Air Quality Data** | PM2.5 levels from 54 stations | 2020–2023 (daily) | [Air4Thai](http://air4thai.pcd.go.th/webV3/#/History) |
| **Global Atmospheric Reanalysis** | Precipitation, Temp, Humidity, Wind, Pressure | 2020–2023 (daily/monthly) | [NOAA Reanalysis II](https://psl.noaa.gov/data/gridded/data.ncep.reanalysis2.html) |
| **Thailand Geo Coordinates** | Latitude, Longitude, Province | Static | [Google Earth Engine](https://earthengine.google.com) |
| **Tourism Data** | Visitors, Revenue (Thai/Foreign) | 2020–2023 (monthly) | [TAT Intelligence](https://intelligencecenter.tat.or.th/articlees/9907) |

---

## 🔧 Data Processing

- **Missing values** were handled using:
  - Forward/backward fill
  - Spatial interpolation (nearby station data)
- **Mapping** station data to provinces using lat/lon
- **Monthly Aggregation** for temporal trends
- **Filtering**: Only 54 provinces retained due to data availability

---

## 📈 Key Visualizations & Insights

### 📌 Revenue vs PM2.5 (National)
- Tourism revenue dropped as PM2.5 levels rose, particularly during high-smog months.
- Peak pollution = **March**, consistently across years.

### 📌 Top Provinces by Tourism Revenue
1. **Bangkok** – 1,407,209 M THB (35.9%)
2. **Phuket** – 707,580 M THB (17.8%)
3. **Chonburi** – 405,820 M THB (9.9%)
4. **Chiang Mai** – 221,418 M THB (5.9%)
5. **Prachuap Khiri Khan** – 105,147 M THB (2%)

### 📌 Chiang Mai Case Study
- Revenue from tourists inversely correlates with PM2.5 during March.
- Strong impact of air quality on local tourism economy.

---

## 🌦️ Weather & PM2.5 Correlation

| Weather Factor      | Correlation with PM2.5 |
|---------------------|------------------------|
| Relative Humidity   | **-0.69**              |
| Precipitation Rate  | -0.45                  |
| Temperature         | -0.42                  |

### Wind Patterns
- March (Max PM2.5): Weak dispersion, stagnant air
- August (Min PM2.5): Stronger wind patterns support better air circulation

---

## 💡 Recommendations & Future Work

- Focus efforts on high-impact months (**March**).
- Promote policies increasing **relative humidity** in urban air.
- Use weather variables to **build predictive models** for PM2.5 surges.
- Design localized **early-warning systems** and **control policies**.
- Encourage **innovations** that modify microclimate (e.g., mist towers).

---

## 📌 Takeaway

PM2.5 is not only a health crisis but also an economic one. A better understanding of meteorological drivers and their influence on tourism can help Thailand strategically tackle air pollution while protecting its vital tourism industry.

---

## 🙏 Acknowledgments

Special thanks to the **Data Universe Hackathon 2024** organizers and data providers.

