import dagshub
dagshub.init(repo_owner='atharva.ai1509', repo_name='mlflow_experiments', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)