# Predictit Data With Airflow And Snowflake

Here is the general outline.

**Data Source:** The data source for this is PredictIt, a marketplace for political predictions.
**Ingestion Method:** You’ll use a Python operator in Airflow and run it in Managed Workflows for Apache Airflow (MWAA) for ease of use.
**Data Storage:** The raw data will be stored in an S3 bucket. From there, the data will be transferred to Snowflake for analytical storage.
**Data Transformations:** There are a lot of ways you can transform data, but you can always use Snowflake’s tasks to perform data transformations.
**Visualization:** Tableau will be used for data visualization purposes.
You’ll use these tools to create a basic function for scraping JSON data from a Predicted API endpoint. He explains the structure of the data and how it will be loaded into S3.

Then you will use Airflow to create a DAG (Directed Acyclic Graph) that defines the workflow for the project. The DAG includes tasks for scraping data and a dummy task called “ready,” which aids in referencing the last task of a DAG.

From there you can take said data to build a data visualization of what is going on in the political landscape. Who is currently taking the lead in terms of bettings lines?

