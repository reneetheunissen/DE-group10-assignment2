# Group10 Assignment2: Data Pipelines

In the deployment directory, the deployment of the application can be found.
In the notebook directory, two Jupyter notebooks can be found. One for Twitter data and one for Reddit data. 
The data can be found in the data directory.

The application can be run by opening a terminal/command prompt and performing the following steps:
1. cd DE-group10-assignment 2/deployment
2. sudo docker-compose build
3. sudo docker-compose up -d
4. sudo docker logs spark-driver-app
5. Open the Jupyter notebook (link in terminal/command prompt output)

Note that the application uses BigQuery and Google Cloud Storage. To run it locally, these values need to be changed
in the notebook. Data can be visualised by connecting Google Data Studio to the BigQuery tables. 
An example of such a visualisation can be found here: https://datastudio.google.com/u/1/reporting/cca53dbe-2bb9-4cc4-a855-fb93dd59c0f9/page/p_b1v3942vpc
