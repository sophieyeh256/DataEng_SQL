# ucb_mids_w205_project_1
Fundamentals of Data Engineering

## Introduction

Project 1 will be an individual project to analyze a sales database.  You will be working in Cloud, specifically in Amazon Web Services, in the official w205 VM, in a docker cluster running one container for Anaconda (Python distro) and one container for Postgres (SQL-based relational database).   You will be writing Python, Pandas, and SQL code in a Jupyter Notebook for your analysis and will be creating data visualizations to enhance your analytics.

Postgres is an open source database that is famous for separating the SQL engine (front end) from the database engine (back end).  Because of this, most modern databases, especially cloud databases, are using the Postgres SQL engine paired with their own back end.  Their back ends can support all levels from small serverless SQL, to mid-range, to gigantic data warehousing.  Some backends are transactional for executing the business, and some are analytical for evaluating the executing the business.  So, the Postgres dialect of SQL is a great addition to your skills set!

## New Skills

* Expand your GitHub knowledge (working on a branch, creating a pull request, etc.)
* Design queries using a Data Model in ERD format (versus hack style SQL based on just looking at tables and guessing)
* Using a secondary dataset to enhance a primary dataset
* Open ended business questions from executives: analyzing, giving an answer, and supporting that answer with data
* Designing an appropriate data visualization to present supporting data
* Functional programming using Python and SQL
* Working in the Linux command line
* Working in the cloud (AWS)
* Working in a VM in the cloud instead of physical computer
* Working in a cluster of Docker containers running inside a VM in the cloud

## Business Case Scenario

A few years ago, a new startup was born: **Acme Gourmet Meals (AGM)**.

The founder of AGM was a sous chef in a 5-star restaurant, named Joy, who had worked her way up from dishwasher to cook to sous chef.  As part of her job, Joy frequently shopped at the high end grocercy stores that featured organic and healtier selections for their food, at premium prices, as the 5-star restaurant wanted only the highest quality ingrediants for their food.  Also, part of her job was to be paid to eat meals on her time off at other restaurants from fast food to other 5-star to see what types of food and quality were being served.  

Joy noticed that most young, single professionals tended to:  
* Eat out frequently, with a mix of mostly casual dining, with some fast food, and occasional 5-star restaurants
* Order delivery at home or work
* Take out for home or work
* Buy frozen pre-made meals and microwave them at home

Joy also noticed that all of these options were typically not very healthy.

Joy had an idea to create a new business.  She would cook healthy, gourmet quality meals and fix them in containers similar to the frozen pre-made meals purchased in grocery stores, except they would be fresh (not frozen) to improve the taste.  She would seek to market them at a local high end grocery store. 

Joy struck a deal with the high end grocery store to setup a small counter there near the entry way. At the counter she would educate the customers about her meals, take orders, and delivery them.  As the business grew, Joy rented space near the store and setup her kitchen there, hiring someone else to staff the counter at the grocery store.  Joy also hired a web developer to develop a website to take orders, handle payments, etc.

After a couple of years or so, the grocery store's corporate office was so pleased with the arrangement, they asked AGM to expand to several other cities.  They selected stores in the areas of town with more young professionals, and/or areas known for more affluence.  They provided funding for a joint venture to allow AGM to setup kitchens near the store and enhance the web and phone app ordering system. In exchange for their investment, they received controlling interest in the business.  Joy stayed on, where she would continue to act as an expert on the food side of the business.

AGM has just finished a very successful year on the enhanced computer systems, and now has a database of sales data for one year.

AGM charges a flat rate of $12 per meal with no minimum. Since it's food that has to be heated before eating, it is not subject to sales tax.  Customers must order by 10am one day in order to pick up the meals the next day. The thinking is that AGM will waste much less food that way.  Customers will have a maximum of one order per day.  

AGM has just hired you as their first full stack data scientist to analyze the sales data. The executives have a lot of questions about how the business is doing and how to improve the business.

## Executive Questions

The executives have some very specific questions, as well as some open ended questions:

**Sales Specific Questions**

* Total sales as a dollar amount
  * for all of AGM
  * by store
  * by month
  * by store and month
  * by day of week
  * by store and day of week

* Total number of sales
  * for all of AGM
  * by store

* Average dollar amount per sale
  * for all of AGM
  * by store

* The Executives have also asked you to provide your best example of a data visualization for one of the above queries.

**Customer Specific Questions**

* Total number of customers 
  * for all of AGM
  * by store
  * by distance from store

* List of customers who have signed up but not bought anything

* Using the secondary dataset, what is the percentage of customers per population
  * at the zip code level?
  * at the city level?

* The Executives have also asked you to provide your best example of a data visualization for one of the above queries.

**Product Specific Questions**

* How many meals were purchased?
  * for all of AGM
  * for all of AGM by meal
  * by store and meal
  * by month
  * by month and meal
  * by day of week and meal
  
* Average number of meals per sale
  * for all of AGM
  * by store

* The Executives have also asked you to provide your best example of a data visualization for one of the above queries.

**Holiday Analytics (open ended)**

How do holidays affect the sales, considering both the actual holiday, and the days before and after the holiday?  Create an executive summary explaining how holidays have affected sales.  You must support your sumary with data, in the form of output of queries, data visualization, etc.  There is a 1 query minimum.

**Best Customer Analytics (open ended)** 

The executives want you to come up with a high level design of a model, in the form of written criteria, to determine who the best customers are.  You do NOT have to code the model.  You do NOT have to give an actual list of best customers. Create an executive summary explaining your model.  You must support your summary with data, in the form of output of queries, data visualization, etc.  There is a 1 query minimum.

**Best Recommendation (open ended)**

The executives would like your best recommendation for the business.  Create an executive summary giving and explaining your best recommendation for the business.  You must support your summary with data, in the form of output of queries, data visualization, etc.  There is a 1 query minimum.
