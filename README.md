# Problem Description and Details
## Udacity Data Scientist Nanodegree Program: Project 1

**Objectives**
1) Pick a dataset
2) Pose at least three questions related to business or real-world applications of how the data could be used
3) Create a Jupyter Notebook, using any associated packages you'd like, to:

    Prepare data:

    - Gather necessary data to answer your questions
    - Handle categorical and missing data
    - Provide insight into the methods you chose and why you chose them
        
    Analyze, Model, and Visualize:
    
    - Provide a clear connection between your business questions and how the data answers them

4) Communicate your business insights:
    - Create a Github repository to share your code and data wrangling/modeling techniques, with a technical audience in mind
    - Create a blog post to share your questions and insights with a non-technical audience

**Outputs:**

There are two deliverables that are required for project completion:
1. A Github repository for the code
2. A blog post of your findings

## Housing price analysis

### In this project, to achieve the above objectives, I analyze the housing data from New England and Wales.

HM Land Registry publish the “Price Paid Data”, detailed data on the sale prices of properties in England and Wales. Datasets are published monthly with transaction-level information, including price, date, location, property type, property age, tenure duration, and transaction type. 
Datasets are available in bulk in multiple file formats and filtered via the Linked Data API. Please use whatever source is most appropriate to your analysis, acknowledging it appropriately in your report.

#### The UK Government's Statistical Datasets are found here:

http://prod.publicdata.landregistry.gov.uk.s3-website-eu-west-1.amazonaws.com/pp-complete.csv

(Contains HM Land Registry data © Crown copyright and database right 2021. This data is licensed under the Open Government Licence v3.0)
It comprehensively covers data from the housing market in England and Wales from 1995 to 2022 and can be used even for commercial analysis.

#### Dataset Description:
A comprehensive description of all the columns in the data can be found here:

https://www.gov.uk/guidance/about-the-price-paid-data

#### Libraries Used:
- pandas for data analysis
- itertools for data analysis
- matplotlib for visualisation
- seaborn for visualisation

#### Code Files
- Jupyter Notebook: House_Price_Analysis_England_and_Wales_Udacity_Project.ipynb

#### In the Jupyter Notebook, the data is cleaned and analyzed to answer the following questions:

- What is the most sold property type in England and Wales?
- Which are the most expensive cities?
- Which property type sold most in the top city?
- What were the effects of crises over the years (the Financial Crash of 2008, Brexit, Covid-19, etc.) on the housing market?
- What are the monthly effects of the sales trends over the years?
- What are the effects when we drill down to the counties? How are the total sales? What is the mean?

#### A Medium blog post with the explaining the top 4 most important insights can be found here:

https://medium.com/@data.camp435/how-to-analyze-the-housing-market-in-england-and-wales-fbf5fa214db4
