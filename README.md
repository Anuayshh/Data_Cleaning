# Data_Cleaning
## AIM
        To read the given data and perform data cleaning and save the cleaned data to a file.
## Explanation
    Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect,
 incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data,
 but rather finding a way to maximize datasets accuracy without necessarily deleting the information.
## ALGORITHM
  STEP 1: Read the given Data
  STEP 2: Get the information about the data
  STEP 3: Remove the null values from the data
  STEP 4: Save the Clean data to the file
## CODE and OUTPUT
### DATA SET:
~~~
import pandas as pd
df=pd.read_csv("Data_set.csv")
print(df)
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
df['aired_on']=df['aired_on'].fillna (df['aired_on'].mode()[0])
df['original_network']=df[ 'original_network'].fillna (df['aired_on'].mode()[0])
df.head()
df['rating']=df['rating'].fillna (df['rating'].mean())
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())
df.head()
df['watchers']=df['watchers'].fillna (df['watchers'].median())
df.head()
df.info()
df.isnull().sum()
~~~
### LOAN DATA:
~~~
import pandas as pd
df=pd.read_csv("Loan_data.csv")
print(df)
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['Loan_ID']=df['Loan_ID'].fillna(df['LoanAmount'].mode()[0])
df.head()
df['Dependents']=df['Dependents'].fillna (df['Dependents'].mode()[0])
df.head()
df['Gender']=df['Gender'].fillna (df['Gender'].mode()[0])
df.head()
df['Education']=df['Education'].fillna (df['Dependents'].mode()[0])
df.head()
df['Self_Employed']=df['Self_Employed'].fillna (df['Self_Employed'].mode()[0])
df.head()
df['LoanAmount']=df['LoanAmount'].fillna (df['LoanAmount'].mean())
df.head()
df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean())
df.head()
df['Credit_History']=df['Credit_History'].fillna (df['Credit_History'].median())
df.head()
df.info()
df.isnull().sum()
~~~
## OUTPUT:
## DATA SET:
## DATA:
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/36da3186-df98-4542-aca2-928420f852e1)




## NON NULL BEFORE:
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/37b7f985-e7a2-4bde-a4e3-c70430f8a653)






## NON NULL AFTER:
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/26c247bf-7660-4523-b1fd-4ebd51bbc316)





## LOAN DATA:
## DATA:
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/59b6ee98-ac8f-4800-8c3d-c84171210f01)


## NON NULL BEFORE:
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/cce41047-f06a-4895-925b-a39970687592)


## MODE:
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/0167bc10-2ca6-47a1-bb50-4dd0f99f87c5)


## MEAN:
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/ab8820e8-abc2-4559-9107-948e5546f528)
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/b6941e43-0a88-4cd0-8b54-ba95d5b72a8b)
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/9557fe41-dae2-4065-99d2-275b723cb89c)
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/37581069-32a1-409a-a57f-0a1a92f8d95c)




## MEDIAN:
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/20153256-a375-4b66-8934-68ede2c7d01f)
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/7632a4b5-390e-4499-ae58-ccd7b8af7c1d)
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/b3fecccd-7c22-480a-baf9-5f307d81d215)


## NON NULL AFTER:
![image](https://github.com/Anuayshh/Data_Cleaning/assets/127651217/e076ed83-efd9-47a6-913b-468627d9ad14)

