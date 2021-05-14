# Data-Science-Class-Assignment-2
Iris classification (using MLflow and Docker )

FROM jupyter/datascience-notebook

RUN pip install mlflow

EXPOSE 5050

docker build -t jupter_notebook_MLflow . --no-cache
docker run -p 8888:8888 jupter_notebook_mlflow
