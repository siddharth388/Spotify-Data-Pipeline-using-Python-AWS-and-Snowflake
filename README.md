# Spotify-Data-Pipeline-using-Python-AWS-and-Snowflake

Technology Stack - 
1. Python
2. AWS Cloud (S3, CloudWatch, AWS Lambda)
3. Snowflake

Python - 
Python is used to pull the Spotify data with the help of Spotify API. The raw spotify data is in the dictionary format which required cleaning with the help of transformation logics using Python

AWS Cloud - 
1. S3 Object Storage - The raw spotify data is stored in the S3 bucket which is sourced with help of AWS Lambda function and Spotify API. S3 is also used to store the data after initial transformation with help of Lambda function.
2. CloudWatch - CloudWatch is used as a trigger to run the Lambda function which is used to extract the Spotify data.
3. AWS Lambda - For this Data Engineering Project I have used 2 Lambda functions. One for Extracting data from Spotify API and other which is used for Data transformation.

Snowflake - 
After all the data transformation data is loaded into Snowflake with the help of Snowpipe. Here by using Snowpipe we establish a connection between S3 bucket and Snowflake in order to pull data from S3 bucket to Snowflake tables.


![1742363494352](https://github.com/user-attachments/assets/829e5ed2-f3d6-4590-b424-85c0f2afb788)
