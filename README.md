#  Real Estate & Housing Market Analysis (Tableau)

An interactive Tableau data visualization project analyzing **21,060 house sales** to uncover pricing trends, property feature impacts, temporal sales patterns, and spatial market dynamics.

---

##  Project Overview
This project provides actionable insights into housing market behavior using Tableau Desktop. By dissecting variables such as living space, bedroom/bathroom configurations, property condition ratings, and location coordinates, this dashboard allows real estate analysts and homebuyers to evaluate market trends effectively.

---

## Key Visualizations & Dashboard Elements

The Tableau workbook (`Real Estate & Housing Market.twb`) comprises 7 analytical sheets assembled into an interactive main dashboard (**`Dashboard 1`**):

*  Price Distribution (`price Distribution`): Binned frequency distribution highlighting price concentration across market segments.
*  Bedroom & Bathroom Distributions: Categorical breakdowns displaying the structural inventory of homes sold.
*  View vs. Condition Matrix (`View&Condation`): A matrix heatmap correlating property physical condition with aesthetic view ratings.
*  Price Trend Analysis (`Line chart`): Time-series chart tracking daily average sale price movements across the dataset timeline.
*  Sales Calendar Heatmap (`Calendar`): Calendar visualization mapping daily sales performance by week and day of the week.
*  Geographical Map (`Map`): Coordinate-based map plotting property locations (`latitude`/`longitude`) across 70 zip codes to identify high-value geographic hubs.

---
##  Dashboard Preview
![Real Estate Dashboard Preview](images/dashboard_preview.png)

##  Dashboard Design & Interactivity

The main dashboard (**`Dashboard 1`**) is structured logically into three visual regions:

### 1. Interactive Control Panel (Left Pane)
* Date Filter: Dropdown filter to isolate specific months/years (e.g., *September 2014*).
* Range Sliders:Interactive range sliders for **Year Built** (`1900–2015`), **Average Sqft Living**, and **Average Sqft Lot**.
* Calendar Heatmap: Highlights active selling days by week number (`Week 36 – Week 40`) and day of the week, allowing users to cross-filter the rest of the dashboard by selecting specific calendar dates.

### 2. Geographic & Time-Series Overview (Top Center/Right)
* Spatial Analysis Map: Geographic map displaying regional price clusters across King County, WA zip codes.
* Daily Average Price Trend: Line chart tracking daily price fluctuations (`Avg. Price` vs. `Day of Month`).

### 3. Feature Distributions & Quality Heatmap (Bottom)
* Price Distribution Histogram: Binned bar chart showcasing price distribution skewness ($400k–$1.2M+).
* View vs. Condition Matrix: Highlight table/heatmap mapping **View Ratings** (*Excellent, Good, No View*) against **Condition Ratings** (*Fair, Good, Very Good*) to evaluate property premiums.
* Structural Distributions:Binned bar charts analyzing inventory by **Bathroom** and **Bedroom** counts.


## Key Business Insights

1. Price Skewness:Most home sales are concentrated between **$300,000 and $600,000**, with a sharp drop-off above $800,000.
2. Optimal Home Configuration: The highest volume of sales occurs in homes with **3 to 4 bedrooms** and **2 to 2.5 bathrooms**.
3. View & Condition Premium: Properties with an **"Excellent" view** command significantly higher total sales values even when the condition is average, proving location aesthetics strongly outweigh minor wear-and-tear.
4. Seasonal / Calendar Peaks: Calendar cross-filtering reveals that weekday sales activity spikes significantly mid-week (Wednesdays and Thursdays) compared to weekends.

 ##  Dataset Summary

* Dataset File: `HouseData.xlsx`
* Total Records: 21,060 home sales transactions
* Time Period: May 2014 – May 2015
* Average Sale Price: $500,270 (Median: $445,000 | Range: $75,000 – $1,495,000)
* Average Living Area: 2,019 sq. ft.
* Geography: King County area (70 zip codes)
