# grpc-sample

This is sample code of gRPC in Python. 

- Necessary packages

```bash
$ python -m pip install grpcio grpcio-tools googleapis-common-protos
```

- Compile `.proto`

```bash
$ python -m grpc_tools.protoc -I./protos --python_out=. --grpc_python_out=. ./protos/helloworld.proto
```

## Run

- Run server

```bash
$ py greeter_server.py
```

- Run client (at another terminal)

```bash
$ py greeter_client.py 
Greeter client received: Hello, you!
```
