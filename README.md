# Databricks client script using Service Principals
Fully automated Databricks client script in Python that does the following:

- Create Databricks Workspace
- Add Service Principal (SPN) to Databricks Workspace with cluster creation rights (SPN does not need admin rights nor any rights on Databricks Workspace control plane)
- Copy notebook to SPN private workspace in Databricks and run notebook on cluster
- Delete SPN from Databricks workspace

Based on https://cloudarchitected.com/2020/01/using-azure-ad-with-the-azure-databricks-api/ from Alexandre Gattiker