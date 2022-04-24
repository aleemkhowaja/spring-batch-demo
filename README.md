# Spring Batch

Spring Batch is the one of the module in Spring which use to process high volume of data from source to destination.

# For Example
You have csv files where all data available and you want to process csv data and dump into the database, then Spring Batch is the best choice to pick.

Before Spring batch, developers was getting one by one record and inserting into db one by one that is very slow process.

# Components in Spring Batch

# Job Launcher
It is an interface and it launch/begin the Spring batch job

# Job
Job launcher will call run method and then Start the job by using Job object.

# Job Repository

It manage the the state of job, either run or success, and then re-run of failed.
It is important to manage the state of data if there is large volume of records.

# Step
 Step is comes from Job  and it combination of 3 components
 There can be multiple Steps and step can have its multiple components like ItemReader, ItemProcessor and ItemWriter 
 # 1 - ItemReader 
      This component is the source like csv, database
    
 # 2 - ItemProcessor
     If some records needs to add some extra functionality then that business logis will be written in this component.
     
 # 3 - ItemWriter ---- Destination 
     This is detination where data will be dump/exported like database, csv.
     
     ![image](https://user-images.githubusercontent.com/11464125/164982909-a1e4ade1-89cc-46db-adc5-15d35fe80ff6.png)

     
     

