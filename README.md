# data-collection
data-collection
### Data collection is a web scrapping and data analysis project where we make use of splinter and bs4 libraries to automate the browsing and extraction of the the following web pages: 
### 1.https://static.bc-edx.com/data/web/mars_news/index.html
### 2. https://static.bc-edx.com/data/web/mars_facts/temperature.html
### Given a recent change in the setup on the local pc a continous error happens with the the browser package of the splinter library not identifying the chrome driver. As a result the output of the code files is not avaliable in the commit, though with the correct setup the code runs without issue.
### The use of a soup object was fundamental for the scrapping as well as the use .html parser to create a structured document to navigate and analyse.
#### Code: 
##### With the Xpert Learning Assistant the following changes/corrections where made:
##### 1. The addition of .reset_index() when calculating the averages and ploting in order to avoid confusion of the original index and to clarify the current state of the Dataframe.
##### 2. The final year lenght calculation with obtaining the average month duration was suggested as a more accurate method considering the size of the data instead of setting a specific date range.
##### "month_ranges = df.groupby('month')['terrestrial_date'].agg(['min', 'max'])" instead of "first_year = df[(df['terrestrial_date'] >= '2013-08-01') & (df['terrestrial_date'] <= '2015-06-18')]"
