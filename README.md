## Initial Motivation
In my role as a Strategic Finance Manager, I am regularly tasked with analyzing large datasets to extract actionable insights that influence strategic decisions. This responsibility sparked my interest in not just reviewing, but also in understanding the intricacies of how data visualizations and dashboards are constructed.

I recognized that by deepening my knowledge in this area, I could enhance my ability to not only interpret data dashboards but also to better communicate with data and product management teams. The process of distilling vast amounts of data into concise, actionable visualizations is fascinating to me. It's a skill that adds immense value by enabling clearer communication and more informed decision-making within our finance team and senior leadership.

Therefore, I decided to expand my expertise into the technical realm of data visualization with Power BI, Tableau and SQL. I aim to bridge the gap between raw data management and strategic financial analysis to drive business growth and enhance strategic decision-making.


# Netflix Unveiled: A Power BI Exploration of Shows and Global Trends

### Motivation:

Given my familiarity with Microsoft tools, I recognized that learning Power BI would be a natural and strategic first step in mastering data visualization technologies.

### Steps: 

I downloaded a Netflix dataset from [kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows?phase=FinishSSORegistration&returnUrl=%2Fdatasets%2Fshivamb%2Fnetflix-shows%2Fversions%2F5%3Fresource%3Ddownload&SSORegistrationToken=CfDJ8CYusWan8yNKiDQcrMXOtQHX_djfNG_zLS6iF0VqGUQjSl8SVQHwEprCmuSuv9vzc_5pV93wrT8OK3JQo3tO5GOoL6JVNb681_4zhs526PsO9fbg90Ilst4ACttQXAbflL6vSph0m_Fac8xoeMz0urCmxVSCz9IMZ1Ke-yaF57TAnKCCvBDADrVDhDy-ujv2i7_9DFhwCTF-OonQUPX2es9XcD56A3rxpskjBjxIBuSfHiv7GNuiBPlavPty6Sjk-kaK_Xp3vIHlOG2LxFOHiQ-unPcEU0ThKqxv1IrnWSqlNZS8DCqFJhMXoPoGEE99T8-zFCxRaFripySkpr2N1P9eNw&DisplayName=Grace+Li) because it was interesting and easy to understand.

I refined the dataset on Excel by segregating names and countries into distinct columns, and by eliminating extraneous spaces and commas. I then split out the dataset into different tables: cast, countries, description, directors, etc. with show ID being the primary key that relates each table to each other.

Next, I imported this data onto MySQLWorkbench. When importing data from Excel, I ran into issue on MySQLWorkbench and figured out need to replace all blank cells with 'NULL'.

I created new relational tables from the original tables by transforming the different columns of names, countries, etc. for each show into individual rows, creating a clearer and more detailed presentation of directors, cast, countries available, etc. per show. I did this by using UNION as shown in the examples below.

Example using the cast table:

<img width="580" alt="Screen Shot 2024-05-10 at 2 42 55 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/c484b89f-1783-4448-aa3b-73fb96243575">

Example using countries table: 

<img width="556" alt="Screen Shot 2024-05-10 at 2 51 05 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/d2af2e98-5178-41e5-9e84-00e22b33092f">

I then imported these new tables onto Power BI and updated the relationship between the tables so that the Netflix Data Titles was the main table with all other tables related to it by show_id as shown below.

<img width="658" alt="Screen Shot 2024-05-10 at 2 54 56 PM" src="https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/73268e70-ee78-476b-9265-011046f5743f">

The final piece was telling a story of this data through visualization. I wanted to offer two views: an overview of Netflix show trends and a deep dive into specs by show. For the visual effects, I went with black and red to mimic the Netflix brand colors. 

For the overview tab, I thought the most relevant metrics to present to an audience who cares about Netflix trends would be shows added by date, shows by rating, top 10 genres and countries available. These metrics will provide the viewer a general insight of Netflix offerings and overall landscape.

For the single title tab, I wanted to present viewers a view of specific shows of interest. Using what topics I would usually search up about a show I was interested in, I decided to display a dropdown title search section and upon clicking it, the viewer can then see when the show was released, the rating, a brief description of the plot, genre, director(s), cast members and countries available.

Learning the PowerBI tool to present what I wanted required a lot video watching and Google searches on topics like how to create different charts, select specific colors and other formatting issues. As suspected though, PowerBI was pretty intuitive for me given I've already worked with other Microsoft tools. For example, I had a general idea of where to click to center tables, filter certain data out and add borders to charts.

### Outcome:



https://github.com/GraceLi14/Grace-s-Data-Visualization-Dashboards-SQL-Tableau-Power-BI/assets/168991262/a03e51f9-d1a5-4eb4-9105-89a34d96d8cd



# Project 2 - Classic Models Data - Mastering Data Integration Leveraging SQL, Excel, and Power BI for Enhanced Analysis and Presentation

### Motivation:

After gaining a foundational understanding of integrating Excel data into Power BI, I utilized Udemy to explore the types of data analysis questions that data scientists typically address for leadership and business stakeholders, and how they utilize SQL, Power BI, and Excel to resolve these queries.

### Steps:

The Udemy course offered access to a database featuring Classic Models with relational tables. It included a series of analytical questions, which I addressed by initially extracting the necessary data using MySQL Workbench, followed by conducting chart analyses in Excel. For a detailed overview of all the questions tackled and the corresponding Excel analyses, please follow this link.

#### Example:

Question:

SQL Pull:

Excel Analysis:


### Outcome:



## Overall what you learned
