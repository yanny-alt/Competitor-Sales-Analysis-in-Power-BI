# Competitor Sales Analysis in Power BI

![](https://github.com/yanny-alt/Competitor-Sales-Analysis-in-Power-BI/blob/main/Images/Competitor%20Sales%20Analysis.jpg)

This project follows the guidance from Datacamp courses to develop a complete Power BI report, starting from data integration from multiple sources, data transformation, modeling, and then visualization.

## Executive Summary

In this project, I tackle a comprehensive sales and market share analysis, focusing on my company's performance internally and externally by comparing it with competing manufacturers. I leverage the power of ETL (Extract, Transform, Load) and data visualization to provide valuable insights for informed decision-making.

## Methodology

To execute this project, I utilized Power BI, a powerful business intelligence tool, which allowed me to connect, transform, and visualize data from multiple sources. The project was structured in several steps:

1. **Data Preparation**: Gathering, cleaning, transforming, and preparing data for analysis.
2. **Data Exploration**: Conducting a comprehensive analysis of Sintec's performance and its competitors' sales and market share.
3. **Dashboard Creation**: Designing a visually appealing and user-friendly sales analysis report using Power BI's interface.

## Dashboard Screenshot

![](https://github.com/yanny-alt/Competitor-Sales-Analysis-in-Power-BI/blob/main/Images/Competitor%20Sales%20Insights%20Dashboard.png)

## Preparing the Data

In this section, I started by exploring and integrating the dataset into Power BI and understanding the challenges faced with the uncleaned data.

### Data Integration and Transformation

1. Loaded all the required data:
   - Sales (US data)
   - `bi_dimensions` (master data with Geography, Manufacturers, Products)
   - International Sales (Canada, Germany, Japan, Mexico, Nigeria)

2. Cleaned and explored the data by:
   - Removing unnecessary columns and replacing null values using the fill-down function.
   - Splitting values by "Columns from example" and ensuring correct data types.

   ![Price](https://user-images.githubusercontent.com/105278875/205037129-07031276-e38d-4cc5-95e0-10b117cb2064.PNG)

3. Transposed tables and appended queries to combine both Sales tables, creating a single table analyzing sales for all countries.

4. Conducted a quick exploratory analysis using Column Profile, Column Statistics, and Value Distribution.

   ![Capture](https://user-images.githubusercontent.com/105278875/205038573-c0ddc014-7629-4e80-9a07-a0579fce2e08.PNG)

5. Filtered Rows to review the last 3 years of data.
6. Created Clustered Column Charts to determine which manufacturers generate the most value.

   ![Revenue by manufacture](https://user-images.githubusercontent.com/105278875/205039032-da27dc2f-b099-4f87-8ae6-baf60ef93742.PNG)

7. Set up relationships between tables.
8. Created new calculations using DAX:

   ```DAX
   Date = CALENDAR(DATE(2017,1,1), DATE(2021,12,31))


## Discovering Business Insights

### Key Business Insights

- Identified major competitors using a top N list.
- Used Stacked Column Charts to see contributions of each manufacturer to total values.
- Visualized Revenue over time using Clustered Column Charts with slicers for interactive exploration.
- Created a hierarchy of Category, Segment, and Product to analyze Revenue in-depth using the Matrix visual.
- Used DAX calculations to show sales growth and the rate at which a product can increase revenue. Applied conditional formatting for better visualization:
  - 0-40%: Red
  - 41-60%: Yellow
  - More than 60%: Light Blue

## Creating a Data-Driven Story

Sintec’s marketing department requested that I keep the report design and UI in line with the company’s standard guidelines. Using the Sunset theme made the report look cleaner and more professional.

- Changed the manufacturer slicer from dropdown to list and added actual logos.
- Uploaded a customized theme, added titles, and changed fonts.
- Used bookmarks and Spotlights to highlight specific visuals and present them in a story.
- Applied advanced AI-based visualizations to make the analysis more robust.
- Added drillthrough functionality to help end users focus on specific entities.
- Completed the analysis and reporting using Power BI's Analyze feature to explain chart trends.

 Here Link to the Interactive Power BI Dashboard [here]( https://app.powerbi.com/view?r=eyJrIjoiNTYzYWE5OTYtYWQ1Zi00N2MxLWE5YmUtMDI4MzJlMjFmMjgwIiwidCI6IjQ5MWM2ZTNhLTA3MjItNDhmMi1iMDFhLWFhMzliODc0MGYxNiJ9)

## Conclusion

- Sintec has a total market share of 38.22% in the USA.
- The highest growth of 18.8% was observed in 2021 compared to the previous year.
- Artisans are generating revenue with over 50% of the market share in Germany.
- Sintec holds 21.15% of the total market share globally.

## Call to Action

For more insights and details on this project, please check out my Medium articles, connect with me on LinkedIn, and visit my portfolio website:

- [Medium](https://medium.com/@yourusername)
- [LinkedIn](https://linkedin.com/in/yourusername)
- [Portfolio](https://yourportfolio.com)
