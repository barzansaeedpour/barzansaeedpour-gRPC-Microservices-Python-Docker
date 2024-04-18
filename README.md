

# gRPC Microservices with Python and Docker

# Table of contents
* [What is gRPC](#what-is-grpc)
* [What is a Microservice](#what-is-a-microservice)
* [How to run this project](#how-to-run-this-project)
* [How to generate the gRPC codes](#how-to-generate-the-grpc-codes)


## What is gRPC

gRPC is a modern open-source high-performance Remote Procedure Call (RPC) framework. It allows efficient communication between services in distributed systems using protocol buffers as its interface definition language and message interchange format

## What is a Microservice

**Microservices** are an architectural and organizational approach to software development. In this model:

1. **Independence and Communication**:
   - Software is composed of **small, independent services** that communicate over well-defined APIs.
   - Each service performs a specific function and is owned by a **self-contained team**.

2. **Benefits of Microservices**:
   - **Agility**: Small teams take ownership of their services, working independently and quickly. This shortens development cycles.
   - **Flexible Scaling**: Each service can be independently scaled to meet demand for specific features.
   - **Easy Deployment**: Services can be updated, deployed, and maintained without affecting other services.

3. **Contrast with Monolithic Architecture**:
   - In monolithic architectures, all processes run as a single service. Scaling and adding features become complex.
   - Microservices break down applications into smaller, specialized components, enabling faster development and innovation.

In summary, microservices enhance scalability, speed, and flexibility in software development, making it easier to innovate and deliver new features quickly.

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
