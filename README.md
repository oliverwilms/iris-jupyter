# iris-jupyter
## Prerequisites
Make sure you have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [Docker desktop](https://www.docker.com/products/docker-desktop) installed.

## Installation: Docker
Clone/git pull the repo into any local directory

```
$ git clone https://github.com/oliverwilms/iris-jupyter.git
```

Open the terminal in this directory and run:

```
$ docker-compose up -d
```

## Load IRIS excel-py-iris Package

```
USER>zpm "install excel-py-iris"
```

## Run python code to read an excel file and populate IRIS global

```
$ docker-compose exec -it iris-jupyter-iris-1 python3 /usr/irissys/mgr/python/iter_excel.py /opt/irisapp/excel/excel_python_iris.xlsx
```
