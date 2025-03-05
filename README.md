
# Connect a Python application on Cloud Run to a Alloy DB for PostgreSQL database

Using [AlloyDB Python Connector](https://github.com/GoogleCloudPlatform/alloydb-python-connector) to securely connect your Python application to your AlloyDB database. 

This repository will demonstrate how to connect a Python application on Cloud Run to a AlloyDB for PostgreSQL database securely with a service account using IAM Authentication.

## Prerequisites : 
Make sure AlloyDB databse flag : alloydb.iam_authentication enabled and follow [AlloyDB Python Connector](https://github.com/GoogleCloudPlatform/alloydb-python-connector)

## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`INSTANCE_CONNECTION_NAME` = "projects/{PROJECT_ID}/locations/us-east4/clusters/alloydb-connector/instances/alloy-db-con"

`DB_USER` = "alloydb-client-service-account@{PROJECT_ID}.iam"

`DB_PASS` = (optional, if followed the `cloudsql.iam_authentication`)

`PRIVATE_IP` = (conditional) if true it will use PRIVATE_IP is not set it will use PUBLIC_IP to connect to Cloud SQL

`DB_NAME` = your-database

