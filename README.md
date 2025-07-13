# dataflow_gcp_employee----
Objective : Load 1000 records of employee from a google cloud bucket to BigQuery using Google cloud dataflow template
Dataflow Template
Dataflow template allow us to package a dataflow pipeline for deployement. Anyone with the correct permissions can then use the template to deploy the package pipeline.
You can create your own custom Dataflow templates or provide pre-built template for common useage.
-----#Steps#-----
1.Creating a Google Cloud Bucket in gcp named Dataflow_demo_bkt01.
![Screenshot 2025-07-03 141627](https://github.com/user-attachments/assets/e0011fad-5e35-4d03-954b-91cdd888b2a2)

2.Create a dataset in BigQuery named employee_set.
![Screenshot 2025-07-03 141016](https://github.com/user-attachments/assets/f52f7352-e0c2-44b7-b3cc-c138ce024084)

3.Add a empty table named employee_tbl.
![Screenshot 2025-07-03 141600](https://github.com/user-attachments/assets/b6fa2ec6-14e8-4118-824e-2631c99dee3a)

4.upload the employee_schema to the gcp bucket.

5.Upload udf.js to the gcp bucket.
![Screenshot 2025-07-03 142538](https://github.com/user-attachments/assets/a07c57f8-2b85-441d-b6e5-1e4d30ec829f)


6.Create a Dataflow template in gcp named dataflow-demo-emp01.
![Screenshot 2025-07-03 142412](https://github.com/user-attachments/assets/97ed21d2-c8e9-4106-b4b1-055c2c31b57e)

7.Set the Source and Target of cloud storage files.
![Screenshot 2025-07-03 142431](https://github.com/user-attachments/assets/48f049e3-50e3-4bd0-b7e9-51cebadea06b)

8.Set the parameter using udf.js
![Screenshot 2025-07-03 142453](https://github.com/user-attachments/assets/2fae7d7e-6f2d-4f0a-83f8-f7b287a06489)

9.Create a dataflow template and start the process.
![Screenshot 2025-07-03 142759](https://github.com/user-attachments/assets/c0f911c5-be18-4cd5-8d67-51c5d2068f60)
![Screenshot 2025-07-03 143026](https://github.com/user-attachments/assets/bea8e481-2c13-4e54-a09d-cddfce8b161b)

10.Check the BigQuery database and employee_tbl is filled by records from the files.
![Screenshot 2025-07-03 143205](https://github.com/user-attachments/assets/9b101f28-6447-4e1b-ac67-87b2e5c0de83)

