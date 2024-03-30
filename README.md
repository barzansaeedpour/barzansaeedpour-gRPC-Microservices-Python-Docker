

# gRPC Microservices with Python and Docker

# Table of contents
* [What is gRPC](#what-is-grpc)
* [What is a Microservice](#what-is-a-microservice)
* [How to run this project](#how-to-run-this-project)
* [How to generate the gRPC codes](#how-to-generate-the-grpc-codes)


## What is gRPC

## What is a Microservice


## How to run this project

* Open two distinct terminals (One for the server and another one for the client)
* In the server terminal:
    * `pip install -r requirements`
    * `python app.py`
* In the client terminal:
    * `pip install -r requirements`
    * `python app.py`

* You will get an output like this:

```
D:\gRPC-Microservices-Python-Docker\client>python app.py
[id: "1"
name: "Barzan Saeedpour"
email: "barzansaeedpour@gmail.com"
password: "123"
]
```

## How to generate the gRPC codes

- In the server terminal:
    - `python -m grpc_tools.protoc -I./protos --python_out=. --pyi_out=. --grpc_python_out=. ./protos/users.proto`
