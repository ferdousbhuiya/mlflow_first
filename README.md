#mlflowexperiments


MYFLOW_TRACKING_URI=https://dagshub.com/ferdousbhuiya/mlflow_first.mlflow
import dagshub
dagshub.init(repo_owner='ferdousbhuiya', repo_name='mlflow_first', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)