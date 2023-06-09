# Data-Cleaning

AIM:

   To read the given data and perform data cleaning and save the cleaned data to a file.

EXPLANATION:

    Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect, incompleted, irrelevant, duplicated or improperly formatted. Data Cleaning is not simply about erasing data, but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

ALGORITHM:

       Step 1: Read the given data.
       
       Step 2: Get the information about the data.
       
       Step 3: Remove the null values from the data.
       
       Step 4: Save the clean data to the file.

CODE:

Data_set.csv

import pandas as pd 

df=pd.read_csv("Data_set.csv")

print(df) 

df.head(10)

df.info()

df.isnull()

df.isnull().sum()

df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0]) 

df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0]) 

df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0]) 

df.head()

df[ 'rating']=df[ 'rating'].fillna (df['rating'].mean()) 

df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())

df.head()

df[ 'watchers']=df[ 'watchers'].fillna (df[ 'watchers'].median())

df.head()

df.info()

df.isnull().sum()


Loan_data.csv

import pandas as pd 

df=pd.read_csv("Loan_data.csv")

print(df) 

df.head(10)

df.info()

df.isnull()

df.isnull().sum()

df['Gender']=df['Gender'].fillna(df['Dependents'].mode()[0]) 

df['Dependents']=df['Dependents'].fillna(df['Dependents'].mode()[0]) 

df['Self_Employed']=df['Self_Employed'].fillna(df['Dependents'].mode()[0]) 

df.head()

df[ 'LoanAmount']=df[ 'LoanAmount'].fillna (df['LoanAmount'].mean()) 

df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean())

df.head()

df[ 'Credit_History']=df[ 'Credit_History'].fillna (df[ 'Credit_History'].median())

df.head()

df.info

df.isnull().sum()

OUTPUT:

Data_set.csv

READ DATA:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/8630fa1b-f3c3-4328-ba0a-eb7b9a4acae7)

NON NULL BEFORE:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/57062715-b524-4e31-9f28-5732f6a579f8)

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/9fa52d46-bc71-42a4-a754-ac564c88c023)

MODE:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/664cc5df-1a17-4958-8330-21fbc2a1e8a0)

MEAN:
 
![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/cdf64a8c-9eb7-4f47-9db4-e932633ad180)

MEDIAN:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/8ab116e7-391f-47d6-b69d-f6eb8788d931)

NON NULL AFTER:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/7fc60fd3-b7fa-4ab9-97b3-e2cd54aa09c5)

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/cc158e27-d424-4896-b9be-083b63859925)

Loan_data.csv

READ DATA:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/a1092b0f-9759-40a1-b06b-a6dca50b7866)

NON NULL BEFORE:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/9f7d7b32-0bf1-43fe-960c-e71f320bf02a)

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/ba9df69f-2206-4a9a-ab04-6c25e44fdc6c)

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/87b8d150-ca73-4766-a5ff-12e54db28831)

MODE:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/7e6f4281-7367-4ace-a19b-de2d782b7b14)

MEAN:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/f55ce0cb-c42b-4ca5-949e-88126446ad93)

MEDIAN:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/fc33bb6c-9e74-49b5-8bf2-db3d161dcc6d)

NON NULL AFTER:

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/bc1ecdd6-4fe8-441a-8878-d75574d6cf5b)

![image](https://github.com/akshitha-ks/Data-Cleaning/assets/123535064/9ce34775-3a94-45af-884a-8b9a813c80c6)

RESULT:

      Thus, the given data is read, cleansed and the cleaned data is saved into file.
