![image](https://github.com/user-attachments/assets/979e4bf8-4872-46b2-b5c3-2dd9aa48c2cf)# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output

import pandas as pd<br>
df=pd.read_csv("/content/SAMPLEIDS.csv")<br>
df<br>
![Screenshot 2025-03-04 205446](https://github.com/user-attachments/assets/98ac9420-d334-46fc-91af-2bd0df00729e)<br>
df.isnull().sum()
![Screenshot 2025-03-04 210028](https://github.com/user-attachments/assets/56422d77-1b6f-42a4-aa99-4f02a6da47a1)
df.isnull().any()
![Screenshot 2025-03-04 210304](https://github.com/user-attachments/assets/2cd982fb-15f0-4510-b09b-cbf665fac6c0)
df.dropna()
![Screenshot 2025-03-04 210432](https://github.com/user-attachments/assets/c8989206-c474-4bb0-a326-7ada03b748f5)
df.fillna(0)
![Screenshot 2025-03-04 210508](https://github.com/user-attachments/assets/bbb96bc8-aae9-4f1c-89a5-6a65dc3dfe8b)
df.fillna(method='ffill')
![Screenshot 2025-03-04 210609](https://github.com/user-attachments/assets/6adfa1ee-f7ba-4c2c-a34c-acc37ed5903e)
df.fillna(method='bfill')
![Screenshot 2025-03-04 210652](https://github.com/user-attachments/assets/94a0fd61-837e-448c-b31e-112a687191c1)




# Result

          Thus we have cleaned the data and removed the outliers by detection using IQR and Z-score method
