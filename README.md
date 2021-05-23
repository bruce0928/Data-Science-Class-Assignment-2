# Data-Science-Class-Assignment-2
Iris classification

# 暫時只完成作業第一部分
第二部分
嘗試以下網址跟著作但還沒找到架不起來的原因

https://mile.cloud/zh/resources/blog/57/%5B%20%E6%89%8B%E6%8A%8A%E6%89%8B%E6%95%99%E5%AD%B8%E6%96%87%20%5D%20%E4%B8%89%E5%88%86%E9%90%98%E5%9C%A8%20GCE%20%E4%B8%8A%E9%83%A8%E7%BD%B2%20Container

https://www.mlflow.org/docs/latest/tracking.html#networking


# 1.dockerfile

## (1)dockerfile內容

    FROM jupyter/datascience-notebook

    RUN pip install mlflow

    EXPOSE 5050

## (2)利用dockerfile在local建立image並建立新的container:

在cmd執行以下指令:
    
    docker build -t jupter_notebook_MLflow . --no-cache
    docker run -p 8888:8888 jupter_notebook_mlflow
