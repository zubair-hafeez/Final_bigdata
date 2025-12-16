Inroduction of the Project

I selected MongoDB for this project because it is a distributed NoSQL database that can handle large volumes of data. I installed Docker locally and ran MongoDB using the command
docker run -d --name mongo -p 27017:27017 mongo:7,
which allowed me to use MongoDB without relying on any cloud service or external setup.

Here I used Python with Jupyter Notebook. First, I collected real-world raw data from the NYC 311 public service API. This dataset contains service requests submitted by New York City residents, such as noise complaints, infrastructure issues, and public service problems. The data is in JSON format and I limited it for 50,000 records with attributes like complaint type, borough, time, and geographic location. I performed data cleaning by removing duplicate records, handling missing values, and converting data types such as dates and numeric fields into the correct format. After cleaning, I imported the processed data into MongoDB.

I then verified the number of rows and columns using MongoDB queries and Python. After that, I used MongoDB aggregation pipelines to generate summarized datasets, including complaint counts by borough, weekly trend analysis, and spatial data preparation for the visualization of the results using Matplotlib, creating bar charts, time-series plots, and geographic density plots. 
