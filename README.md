# DataCleaning
# AIM
    To read the given data and perform data cleaning and save the cleaned data to a file.
# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect,
incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data, but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
STEP 1: Read the given Data STEP 2: Get the information about the data STEP 3: Remove the null values from the data STEP 4: Save the Clean data to the file

# CODE and OUTPUT
# DATA SET:
~~~import pandas as pd
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
# LOAN DATA:
~~~import pandas as pd
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
# OUTPUT:
# DATA SET:
# DATA:
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/e7592ff2-f33b-4165-adb5-2bc085f1e854)


# NON NULL BEFORE:
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/161c924e-69b4-4243-af81-25351e77d9ad)


# NON NULL AFTER:
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/54b21dd3-145a-4ada-af97-c89809c9301e)


# LOAN DATA:
# DATA:
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/a51c6006-5ecb-4ca6-9f29-11d717b03649)


# NON NULL BEFORE:
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/1b48f057-b32d-472e-a147-9001606a55a0)


# MODE:
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/53904770-902c-4ae1-8c61-e82c2c028ec3)


# MEAN:
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/d827f12b-665c-44b8-b157-2737e47beb66)
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/ce2c475d-e774-4542-8395-6e5bdddd1d46)
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/8f2f36d5-0f0b-42f5-b686-a39d26ad2e34)
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/81f872ef-4275-45d9-b62d-5401f635f3ab)




# MEDIAN:
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/6dba4ddf-57b3-4be3-8471-b4778553182d)
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/b1f95b38-efd4-4d4c-bf20-64bf626a73c7)
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/48a40e9c-fc33-452a-b9e2-39d5bc20a841)



# NON NULL AFTER:
![image](https://github.com/Leela1822/DataCleaning/assets/106167639/72e8501c-c303-4914-9f99-f10110a060e3)
