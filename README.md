# MLFLOW Experiments 

MLFLOW_TRACKING_URI=https://dagshub.com/Dhiraj1312/MlLFLOW.mlflow \
MLFLOW_TRACKING_USERNAME=Dhiraj1312 \
MLFLOW_TRACKING_PASSWORD=8ed6890d7815e6412aa2e3b7d7c4d822e4b24abc \

import dagshub
dagshub.init(repo_owner='Dhiraj1312', repo_name='MlLFLOW', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)