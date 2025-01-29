# ETL using Snowflake

I created two tables LANDING_FINANCE_TABLE AND STAGING_FINANCE_TABLE and one stream LANDING_TO_FINANCE_TABLE.
![p11](https://github.com/user-attachments/assets/52af5b1b-e785-4385-a7ac-daaccf492e83)

I created a task named TO_APPEND_FINANCE_TABLE
![p12](https://github.com/user-attachments/assets/ceaa074e-c003-405e-bf93-c16cf7a97251)

Here I created a storage integration for the stage 
![st](https://github.com/user-attachments/assets/4a5c0fed-d5c9-4377-a2ea-c72c86f36ce4)

Then Provided permission of Storage Blob Data Contributor 
![st1](https://github.com/user-attachments/assets/5997dec2-65fa-47a6-aa2d-ae09558c5629

Created a CSV file format and stage AZURE_ETL_STAGE
![fs](https://github.com/user-attachments/assets/6d42c48b-f758-4cf0-8238-44455835224d)

Here I tried copying data manually from Azure Blob Storage to our tableLANDING_FINANCE_TABLE and it succeeded 
![cp](https://github.com/user-attachments/assets/b48df6d9-dd41-4f1a-a0e2-a57d127688cd)

I created one Notification Integration named SNOWPIPE_EVENT
![nt](https://github.com/user-attachments/assets/2dbfff0e-4f3a-47eb-a19d-9c2a9e4bae45)

Then provide Storage Queue Data Contributor role in Azure 
![nt1](https://github.com/user-attachments/assets/defb436f-d366-4891-a77b-c520c47b792d)

Created a queue eventqueuefroblob 
![nt2](https://github.com/user-attachments/assets/25c02523-bc1d-4c5a-a1b9-034b98589aa8)

Created a Snowpipe AZ_PIPE
![snowpipe](https://github.com/user-attachments/assets/d21e0378-b38a-452e-b4ca-74a363a6b285)

Below are snip testing of ETL
![1](https://github.com/user-attachments/assets/30713fb8-5bbe-4a98-8748-2b0eea41ad2e)
![2](https://github.com/user-attachments/assets/57325198-1d74-40fa-8e55-b7c882d17542)
![3](https://github.com/user-attachments/assets/db7e9c71-a420-4793-8e5d-e0c0e69d0507)
![4](https://github.com/user-attachments/assets/5ea2c1f4-3d0c-41d9-94b2-d241242395f9)
![5](https://github.com/user-attachments/assets/dea6e1c1-504f-42b3-b1e7-315aba89fc5d)
We can see that data has been copied to LANDING_FINANCE_TABLE and STAGING_FINANCE_TABLE
![6](https://github.com/user-attachments/assets/e65546e5-9310-4f00-afe0-228945247d07)
![7](https://github.com/user-attachments/assets/71e2fd64-78af-402a-b457-476dedc8a992)
Here I connected the data source to the Finance Dashboard
![image](https://github.com/user-attachments/assets/ba71fdda-fb48-40a6-bf0e-369c5abe88f6)
![image](https://github.com/user-attachments/assets/3f4391cf-763f-41bf-9a76-a99b18d7e80d)
![image](https://github.com/user-attachments/assets/daeb2f00-d9fd-4536-828f-109be66984fe)
![image](https://github.com/user-attachments/assets/27a70550-1007-4100-bdc8-4cf333bf8d73)
![image](https://github.com/user-attachments/assets/01bce6cc-3c11-419e-b990-999ad3edbdeb)
Here we can see data for 2021-01-01
![image](https://github.com/user-attachments/assets/df29d00d-2d8f-4a2e-87f8-b5e1f5b6bfc6)








