# Brand-Association-Analysis

This is one of my first projects in text analytics and hence applied only limited techniques. As we proceed in the learning, more comprehensive techniques and analysis were done.

![image](https://user-images.githubusercontent.com/26767610/225181001-b8de4996-39f3-4e31-b693-7cf16fb2b3ed.png)

Edmunds is a popular online user forum in the US where people discuss about car brands, features etc. The aim here is to use this user generated content to perform a car brand analysis and derive insights. For our analysis, we decided to focus on the mid-size sedan forum.

### Project Objectives:

Goal is to perform a competitive analysis of the entry level luxury car market in the USA by scraping "Edmunds" car-forum for social media conversations. Then recommend actionable insights based public perception of car brands.

### Approach

1. Write a scraper using Selenium to fetch messages posted in Edmunds.com discussion forum. We scraped around 5000 posts from the mid-size sedan forum.
2. Identify the top 10 brands by frequency.
3. Calculate lift ratios for associations between the brands and show them on a multi-dimensional scaling (MDS) map.
4. Identify the most frequently mentioned attributes of cars in the discussions.
5. Identify the attributes that are most strongly associated with certain brands.
6. Identify the most aspirational brand.
7. Based on inferences, formulate advices for i) product manager, and (ii) marketing/advertising manager of these brands.

### Insights

#### Multi Dimensional Scaling (MDS) plot

Brands discussed together frequently are closer in below plot.

![Screenshot 2023-03-14 210443](https://user-images.githubusercontent.com/26767610/225186291-fa8e1308-375a-4398-b0cb-24e9f3ca28ae.jpg)

1. We see that the lift ratios are high for (Nissan, Toyota), (Honda, Toyota) and (Acura, Infiniti). This is evidence that people have similar perception about these brands. These companies can target the users of the other two brands as they would be more likely to switch, if offered slightly better price point or features. Being japanese brands, it makes sense that customers think of these three brands in close association.
2. We see that the Infiniti, Acura and Audi also have high lift values among each possible pair. This gives us another market segment which these brands can target when advertising for their entry level luxury car models. 

#### Brand-Attribute association

![image](https://user-images.githubusercontent.com/26767610/225184629-4842ba19-a324-4f9e-b6a9-57d4872a18ca.png)

1. From the lift calculations in the table above we see that Cadillac is most associated to luxury. However, it is peculiar to note that Volvo has the most mentions associated to luxury. This maybe because Volvo customers are most likely to aspire and hence switch to luxury brands.
2. We see that Ford is least mentioned when AWD is discussed, this gives the company a possible area to improve upon so as to draw in more customers who are looking for AWD.
3. We see that Infiniti is mentioned the most when people talk about the price of a car, which is expected due to the Infiniti's value-for-money cars.
4. When it comes to engine, Nissan is the most talked about brand. They can leverage this feature to differentiate itself from its competitors. 


#### Aspirational brands

![image](https://user-images.githubusercontent.com/26767610/225184314-0fd2e11d-250e-4962-a5ae-f4f229220a40.png)

Audi is the most aspired brand in this dataset as per the attributes we focussed on (engine, luxury, performance, price, AWD). From this we can infer that Audi has positioned itself well with car enthusiasts and customers in general. Audi can pull in a lot of customers from other brands positioning themselves as better in the attributes we measured. 
