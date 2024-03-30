



## Server:

- python -m grpc_tools.protoc -I./protos --python_out=. --pyi_out=. --grpc_python_out=. ./protos/users.proto

## How to run:

* Open two distinct terminals (One for server and another one for client)
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
