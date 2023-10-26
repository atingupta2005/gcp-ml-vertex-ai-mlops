
# /02 - Vertex AI AutoML/readme.md

This series of notebooks will introduce [Vertex AI AutoML](https://cloud.google.com/vertex-ai/docs/start/automl-model-types) with a focus on Tabular data Classification Methods.

Vertex AI AutoML accelerate the workflow of creating an ML model by preprocessing the data and choosing model architectures for you, even testing multiple and creating ensembles to achieve a best model.  This is available for ML models on text, image, video, and tabular data.  

**Prerequisites**
- [00 - Setup.ipynb](../00%20-%20Setup/00%20-%20Environment%20Setup.ipynb)
- [01 - BigQuery - Table Data Source.ipynb](../01%20-%20Data%20Sources/01%20-%20BigQuery%20-%20Table%20Data%20Source.ipynb)

---
## AutoML Services

[AutoML](https://cloud.google.com/vertex-ai/docs/beginner/beginners-guide) is a service on Vertex AI that creates custom models from users data.  The data source for AutoML jobs is a [Vertex AI managed dataset](https://cloud.google.com/vertex-ai/docs/datasets/overview).  These managed datasets are links to actual data locations in GCS or BigQuery. The data is not imported so each training job that uses them will always grab a current version of the data source. When creating a dataset, the location selected needs to match the location of the linked data (like `us-central1` for example).  AutoML training jobs use these datasets as inputs.  The AutoML service availability by region should be reviewed to make sure it is available in the data location - [feature availability](https://cloud.google.com/vertex-ai/docs/general/locations#vertex-ai-regions).

When using [AutoML from BigQuery ML](https://cloud.google.com/bigquery/docs/reference/standard-sql/bigqueryml-syntax-create-automl) a Vertex AI managed dataset is not required.  Instead, the BigQuery locations should be checked for AutoML availability via [this table](https://cloud.google.com/bigquery/docs/locations#bqml-loc) of BigQuery ML resource locations.
