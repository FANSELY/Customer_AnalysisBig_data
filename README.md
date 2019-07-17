# Customer_AnalysisBig_data
I- Big data project of cutomer analysis using Apache PIG

1)download web file of customer analysis using the link 
2)Put both the csv files in Hadoop cluster
3)Register the jar file
4)Now execute the PIG command one by one

command_1)find the top 5 best customer
command_2)Which month saw the largest number of cancellations of the accessories due to poor quality of work?
order 3) The top 10 countries that come to order from your e-bisuness website

analysis.jar is a mapreduce function that indicates which clients have visited your destination.


II- Marketing Analysis


+ Batch analytics 
+ ML: supervised learning model with Classification 
+ MapReduce job to generate a list of customer who are not likely to respond to offer 


### Solution : 
+ Classification machine learning model - Binary classification
+ Tree based learning approach 
+ Finding the right dataset : age, income, gender, folder, response 
+ Train classification model - Scoring 


#### Building machine learning model with BigML 
+ BigML: web-based tool, data processing is done in the cloud 

#### Model building steps 
1. Upload data file : responsedata.csv 
2. Create dataset with data file 
+ See the summary chart of it 
3. Build classification model 
+ Browse decision tree created by BigML 
+ As shown from Prediction path: Age and Income is the 2 most important factor 
+ Model summary report 
<img src="./img/4.png">
4. Download classification model 
+ Make selection of data from database 
+ Use the classification model to predict 
+ Scoring process 
5. Run the model using MapReduce on Hadoop for scoring
+ Run the model on Hadoop 
+ MapReduce job  


#### Run the project on Hadoop with MapReduce 
+ `mvn package`
+ Start hadoop service `/usr/local/hadoop/sbin/start-all.sh`
+ `hadoop jar marketing-analysis-1.0-SNAPSHOT.jar ResponsePrediction /marketing-analysis/data/inputdata.csv /marketing-analysis/output`


#### Screenshots project 
<img src="./img/1.png">
<img src="./img/2.png">
<img src="./img/3.png">
<img src="./img/4.png">
<img src="./img/5.png">
<img src="./img/6.png">
