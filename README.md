# Data-Science-Class-Assignment-2
Iris classification

1.dockerfile

(1)dockerfile內容

    FROM jupyter/datascience-notebook

    RUN pip install mlflow

    EXPOSE 5050

(2)利用dockerfile在local建立image:

在cmd執行以下指令:
    
    docker build -t jupter_notebook_MLflow . --no-cache
    docker run -p 8888:8888 jupter_notebook_mlflow
