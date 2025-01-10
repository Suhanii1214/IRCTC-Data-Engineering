## IRCTC Data Engineering Project

- In this project, the real-time ticket booking data is synced to Big Query.
- I have used a Python script which generates mock data and publishes it on to the **Pub/Sub**
![Screenshot (651)](https://github.com/user-attachments/assets/811ce59d-d787-4802-930f-8a034c1814cd)

- Next the Dataflow performs the following:
  -- Read data from Pub/Sub
  -- Apply python UDF (user-defined function) to transform the data
  -- Check for any fault tolerance
- Google Storage Bucket stores the transform-udf.py file which will be used to register the transformations to Dataflow
  ![Screenshot (655)](https://github.com/user-attachments/assets/d8fbe95c-12a3-4516-8538-faa50c226472)

- Finally the Dataflow performs the Job of writing the data into Big Query
![Screenshot (652)](https://github.com/user-attachments/assets/c7be2f9b-9b93-4124-a1a5-0008d480105b)
![Screenshot (653)](https://github.com/user-attachments/assets/1224dc0c-81cf-4fc2-a96b-ef3412f1ba53)
![Screenshot (654)](https://github.com/user-attachments/assets/f4221219-f22d-422e-ae26-6cf83c6e1850)
![Screenshot (650)](https://github.com/user-attachments/assets/8c7a9910-e108-4abb-a429-3a6b4172b630)
