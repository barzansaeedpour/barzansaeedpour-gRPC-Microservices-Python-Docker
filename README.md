



## Server:

- python -m grpc_tools.protoc -I./protos --python_out=. --pyi_out=. --grpc_python_out=. ./protos/users.proto

## How to run:

- python app.py