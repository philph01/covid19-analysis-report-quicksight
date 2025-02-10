# COVID-19 Analysis Report Visualizations Using QuickSight

## Project Description
This repository contains an analysis and visualizations of global COVID-19 data using **AWS QuickSight**. The project leverages publicly available data from **Our World In Data** to create interactive and insightful visual reports on COVID-19 trends across different regions.

The analysis includes:
- COVID-19 case trends over time (from 2020 to 2025)
- Cases per Region
- Average Cases per Country

![Alt text](/screenshots/screenshot01.png?raw=true "Screenshot of Report")

You can view the full analysis and visualizations in the **PDF format** here:
[Download COVID-19 Visuals Report (PDF)](COVID_Cases_Analysis_2025.pdf)

## Dataset
The dataset used in this project is sourced from **Our World In Data**, which provides daily updates on COVID-19 statistics across the globe. The dataset includes the following key data points:
- Daily confirmed cases
- Daily deaths
- Daily recoveries
- Total cases, deaths, and recoveries by country
- COVID-19 vaccinations data

You can access the original dataset at: [Our World in Data - COVID-19 Dataset](https://github.com/owid/covid-19-data)

## Technologies Used
- **AWS QuickSight**: Used for creating interactive visualizations and dashboards.
- **Our World In Data**: Source of the COVID-19 dataset.
- **Amazon S3**: Used for storing the dataset and connecting it to QuickSight.
- **CSV/Excel**: Format of the dataset used for analysis and visualization.

## Getting Started

Follow these steps to set up and view the project on your own AWS account.

### Prerequisites
- AWS Account with access to AWS **QuickSight** and **S3**.
- Basic knowledge of AWS services (QuickSight, S3, IAM roles).

### Steps to Replicate the Project
1. **Download the Dataset**: 
   - Go to [Our World in Data COVID-19 Dataset](https://github.com/owid/covid-19-data) and download the CSV/Excel file for the analysis you want to perform.
   
2. **Upload the Dataset to S3**: 
   - Log into your AWS console and navigate to **S3**.
   - Create a new S3 bucket (or use an existing one) and upload the dataset you downloaded.
   
3. **Set Up AWS QuickSight**:
   - Open **QuickSight** from your AWS console.
   - Create a new **Data Source** in QuickSight, select **S3**, and provide the S3 URI to the dataset. Optionally, you can provide a manifest.json. I've included the file in this repository as well.
   
4. **Create Visualizations**:
   - Once the data is imported, use **QuickSight** to create interactive visualizations such as time series charts, bar graphs, and heat maps.
   - Save the analysis as a **Dashboard** to share your findings.
   
5. **Access the Report**:
   - You can share the dashboard via AWS QuickSight or embed it into a web application or export it to PDF file as a static report.

## Visualizations

This project includes various visualizations to explore COVID-19 data trends:

- **Global Cases Over Time**: A line chart showing the progression of confirmed cases globally.
- **Cases by Continent/Region**: A bar chart comparing total cases across countries by year.
- **Average Total Cases by Country**: A stacked bar chart displaying the deaths and recoveries for each country.

Here is an example of one of the dashboards created:
![COVID-19 Dashboard](link_to_screenshot_or_gif)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
