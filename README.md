## Initial Motivation
As a Strategic Finance Manager, I regularly analyze large datasets to derive actionable insights for strategic decisions. This sparked my interest in how data visualizations and dashboards are constructed, leading me to deepen my understanding in this area. 

By mastering these skills—using tools like Power BI, Tableau, and SQL—I can better interpret data, communicate with data and product management teams, and distill complex data into clear visualizations. 

This enhances decision-making across our finance team and senior leadership, bridging the gap between raw data management and strategic financial analysis to drive business growth.


# Project 1 | Netflix Unveiled: A Power BI Exploration of Shows and Global Trends

### Motivation:

Given my familiarity with Microsoft tools, I recognized that learning Power BI would be a natural and strategic first step in mastering data visualization technologies.

### Steps: 

I downloaded a Netflix dataset from [kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows?phase=FinishSSORegistration&returnUrl=%2Fdatasets%2Fshivamb%2Fnetflix-shows%2Fversions%2F5%3Fresource%3Ddownload&SSORegistrationToken=CfDJ8CYusWan8yNKiDQcrMXOtQHX_djfNG_zLS6iF0VqGUQjSl8SVQHwEprCmuSuv9vzc_5pV93wrT8OK3JQo3tO5GOoL6JVNb681_4zhs526PsO9fbg90Ilst4ACttQXAbflL6vSph0m_Fac8xoeMz0urCmxVSCz9IMZ1Ke-yaF57TAnKCCvBDADrVDhDy-ujv2i7_9DFhwCTF-OonQUPX2es9XcD56A3rxpskjBjxIBuSfHiv7GNuiBPlavPty6Sjk-kaK_Xp3vIHlOG2LxFOHiQ-unPcEU0ThKqxv1IrnWSqlNZS8DCqFJhMXoPoGEE99T8-zFCxRaFripySkpr2N1P9eNw&DisplayName=Grace+Li) and refined the Excel dataset by organizing names and countries into separate columns and removing extraneous spaces and commas. 

Subsequently, I divided the data into distinct tables—such as cast, countries, description, and directors—linked by the show ID as the primary key. Refer to [Netflix Project
/DataImport_MySQLWorkbench folder](https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/tree/main/Netflix%20Project/DataImport_MySQLWorkbench) to see resulting Excel sheets.

Next, I imported this data onto MySQLWorkbench. I created new relational tables from the original tables by using UNION as shown in the examples below. Refer to [Netflix Project/Creating Relational Database_SQL Code folder](https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/tree/main/Netflix%20Project/Creating%20Relational%20Database_SQL%20Code) to see all SQL codes used to create these relational tables.

Example using the cast table:

<img width="580" alt="Screen Shot 2024-05-10 at 2 42 55 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/c484b89f-1783-4448-aa3b-73fb96243575">

I then imported these new tables onto Power BI and updated the relationship between the tables so that the Netflix Data Titles was the main table with all other tables related to it by show_id as shown below.

<img width="658" alt="Screen Shot 2024-05-10 at 2 54 56 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/73268e70-ee78-476b-9265-011046f5743f">

The final piece was telling a story of this data through visualization. I wanted to offer two views: an overview of Netflix show trends and a deep dive into specs by show. For the visual effects, I went with black and red to mimic the Netflix brand colors. 

### Outcome:



https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/a03e51f9-d1a5-4eb4-9105-89a34d96d8cd



# Project 2 | Classic Models Data - Mastering Data Integration Leveraging SQL, Excel, and Power BI

### Motivation:

After gaining a foundational understanding of integrating Excel data into Power BI, I utilized Udemy to explore the types of data analysis questions that data scientists typically address for leadership and business stakeholders, and how they utilize SQL, Power BI, and Excel to resolve these queries.

### Steps:

I used an Udemy course that had a series of analytical questions and a database featuring Classic Models with relational tables. 

I tackled these questions by first extracting the necessary data using MySQL Workbench, then by conducting chart analyses in Excel. For a detailed overview of all the questions tackled and the corresponding Excel analyses, please follow this [link](https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/tree/main/Classic%20Models%20Project).

#### Example Problem:

Question:

<img width="737" alt="Screen Shot 2024-05-12 at 1 17 50 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/98914603-29ec-4972-a443-feb1570e754c">

SQL Pull:

<img width="841" alt="Screen Shot 2024-05-12 at 1 18 58 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/75c112e2-c19d-4267-92ae-873918ff7143">


Excel Analysis:

<img width="1195" alt="Screen Shot 2024-05-12 at 1 27 08 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/64eb9fdb-01ba-4cc4-9af6-df78e936aadc">
<img width="1070" alt="Screen Shot 2024-05-12 at 1 27 23 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/07d703f5-1057-4150-be95-a52411cb91ed">

Similar to the Netflix project, I then transformed the analyzed data into a dashboard on PowerBI.

### Outcome:

https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/ff81d08b-cb8c-4a82-9820-fbf713f3aa19

# Project 3 | Exploring Ecomobility - Navigating Bike and EV Industries with Tableau Dashboards

### Motivation:

The final component of this data visualization journey involves mastering Tableau. 

I aimed to explore bike and EV industries because they are related to micromobility. I can utilize Tableau to visualize KPIs, trends, and categorizations similar to those critical in my field. 

### Steps:

For EV data, I used [this dataset](https://catalog.data.gov/dataset/electric-vehicle-population-data).

For bike data, I used [this dataset](https://www.kaggle.com/datasets/prepinstaprime/europe-bike-store-sales).

I then created a Tableau Public account and took a look at dashboards created by other users. 

I aimed to create impactful visualizations tailored for business stakeholders, utilizing proven methods that resonate within the micromobility industry.

### Outcome:
[My Tableau Public](https://public.tableau.com/app/profile/grace.li4022/vizzes)

<img width="1356" alt="Screen Shot 2024-05-12 at 9 56 34 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/623903d8-e7c9-44f5-b5e8-9228acf68b1d">

<img width="992" alt="Screen Shot 2024-05-12 at 9 57 34 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/13bdfcb4-0889-482f-82d5-ceae41a6d794">

## Overall Lessons Learned

Much of my time spent on data extraction from SQL and loading it into various visualization tools involved troubleshooting software issues. This experience enhanced my understanding of common technical problems and how to address them. 

For instance, I learned that MySQL Workbench struggles with importing blank cells from Excel, prompting me to replace these cells with NULL values to ensure smooth data integration. 

This knowledge will enable me to more effectively communicate with data and software engineering teams, helping to streamline the entire process from backend data extraction and refinement to frontend visualization and decision-making.

Additionally, mastering these tools has given me the ability to increased operational efficiency through automation, reducing manual data handling and freeing up more time for strategic planning and analysis.
