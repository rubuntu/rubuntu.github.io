# A journey towards (Driverless) AI

I have been asked how it should be done to enter to the Data Science area.  
There is no single learning path.

_**The short answer:**_  
 I recommend reviewing high school and university mathematics:  
- Linear algebra  
- Calculus  
- Statistics  
- Then take a Data Science course in a MOOC.
- Attend Data Science Meetups & Conferences  

As a programming language you can learn R or Python, but also tools with GUI such as KNIME, RapidMiner, IBM SPSS Modeler, among others.  

_**The long answer:**_  
A long answer is to tell you about my journey to Data Science.  
First of all I do not consider myself an expert, but rather a person who seeks to learn continuously.  
Also, I consider myself a technical person with interests in business. My academic education is a BA in Computer Science, and I am studying an MBA and I have yet to resume a master's degree in computer science.  
Although today I work in the area of Data Science, I had the opportunity to rotate to other areas like: Business/Marketing and Risks, which gave me a broader view of the organization.  
My first contact with Data Science was when I was taking the aforementioned master in computer science course, with Data Ware Housing and KDD / Data Mining subjects, which sparked my interest in that area.  

_**Data Warehousing & BI**_  
In the mean time I took a job opportunity at Vision Banco, a bank in my country Paraguay, where I joined an area specialized in Data Warehousing & Business Intelligence (BI).  
This analytical initiative works in the organization as a bridge of the IT area with the other areas of the company and as a consolidated source of information. The methodology of Ralph Kimball was adopted for the construction of the Data Warehouse. The suite of BI tools that was adopted is IBM Cognos, and It's being used in Reports, OLAP Cubes, Interactive Dashboards, Planning applications and Balanced Scorecards (applying the concepts of Robert Kaplan).  
The ETL processes (Extraction, Transformation and Loading) is made with the open source software Pentaho Data Integration, today part of the Hitachi Vantara suite. 

_**Predictive Analytics**_  
In 2012, an external consultancy was contracted for the development and accompaniment of the deployment of a _"Credit Scoring"_ model. This predictive model, was developed using IBM SPSS using the Logistic Regression algorithm. By accompanying the development of this credit scoring model, we learned -how to- and incorporated in our organization the next level in the Descriptive Analytics (What?) and of Diagnosis (Why?), when starting to do also Predictive Analytics (What will happen?) And Prescriptive (How to make it happen?).  

_**Big Data Pilot**_  
In 2014 we did a pilot project of Big Data: Sentiment Analysis in Social Networks. The infrastructure was contracted on the cloud and we used NoSQL Redis and MongoDB clusters, where "tweets" of the social network Twitter were processed for monitoring of the bank's image. In the text mining process, the Naive Bayes algorithm was used, which despite being simple, worked very well.  

_**Data Science**_  
In the mean time, the bank's *Data Warehouse/BI* area was renamed to *Data Science*.  
From 2015 to date, within the organization, predictive in-house models with more advanced algorithms were developed: Random Forest, GBM, XGBoost, Deep Learning and assemblies with these algorithms, and deployed into production using openscoring.io (models in PMML format) and lately, H2O.ai.  

_**H2O.ai**_  
How did I discover H2O.ai ?, through blogs from data science, where every time I saw more and more mentions.  
At that time I used to make models in R using Random Forest, but building a model with this algorithm with traditional R libraries could take hours. When I first evaluated H2O, building the same model lasted minutes on the same hardware! Why? Because H2O is optimized and uses all the cores of multicore equipment present in any desktop today. Another advantage of using H2O is that the code that could run on a laptop is the same to run in a cluster scaling to Big Data!  
From there we started to make the transition to H2O as the main platform to develop machine learning solutions in the organization.  

_**Driverless AI**_  
A little over a year ago, I had the opportunity to evaluate a new proposal for H2O.ai: Driverless AI, a platform that automates much of the data science process by doing feature engineering, training and model assembly, along with the possibility to generate pipelines for the deployment of the final model and models for the interpretation of it.  
In order to do a Driverless AI proof of concept, I rent a VM with a GPU on the cloud and participated in a data science contest organized by AnalyticsVidhya.com: "Data Science Hackathon: Churn Prediction", obtaining the 8th place!  
I wrote about it in the following post: https://www.linkedin.com/pulse/how-get-eighth-place-data-science-competition-using-driverless-diaz/  
This awesome result is because Driverless AI uses the expertise of "Kaggle Grand Masters in a Box" See https://www.h2o.ai/blog/kaggle-grand-masters-recipes-production-ready-clicks/  
The proof of concept served to demonstrate the many possibilities and advantages of using Driverless AI.  

_**IBM Power System AC922 + Driverless AI**_  
In the mean time, when Vision Banco accepted to acquire the IBM Power System AC922 hardware -with with POWER9 CPUs and NVIDIA Volta GV100 GPUs- to support its initiatives for machine learning (ML) and artificial intelligence (AI), it was also acquired the H2O Driverless AI software.  
We started using H2O Driverless AI for critical use cases: propensity to buy, default prediction, credit scoring, etc.  
The new developments of predictive models of use cases with classification and regression are already being done with Driverless AI, and we plan to use it with time series forecasting and natural language processing (NLP) projects.  
By using Driverless AI on IBM Power System AC922, we have been able to build our ML/AI solutions in less time, with improved quality and accuracy.

**PS:** I have been honored to be Speaker at H2O World San Francisco (http://h2oworld.h2o.ai/h2o-world-san-francisco/), to talk about the ML/AI journey at Vision Banco with H2O Driverless AI on IBM POWER9-based systems with GPUs.  
If you're in San Francisco those days, let's meet there!  


**PPS:** Take a look at my open source project: H2O.ai's open source Mojo Model & Driverless AI Mojo Pipeline REST web service for real-time scoring. https://github.com/rubuntu/h2o_scorer