# gRPC (Google Remote Procedure Call) Golang

[This code's has been inspired from from the grpc.io site.](https://grpc.io/docs/languages/go/quickstart/)

POC of a gRPC project in Golang 🐿

## Explanation comparing to a REST API

- `helloworld/helloworld.proto` file is like a **Controller** class. It's where you will configure the _endpoint_ (in gRPC, those are method names) and the DTO for request and response.

- `greeter_server/main.go` file is like a **Service** class. It's where you will implement all the method business rules.

- `greeter_client/main.go` file is an example of a programatic way to consume a gRPC method from the `helloworld.proto` and `greeter_server/main.go` files.

## Run

### Hello World

From the `root` directory:

Run the server:

```bash
go run greeter_server/main.go
```

From another terminal window, run the client:

```bash
go run greeter_client/main.go
```

## Usage

### Using BloomRPC ([https://github.com/uw-labs/bloomrpc](https://github.com/uw-labs/bloomrpc))

Importing the `helloworld/helloworld.proto` file.

<img width="1324" alt="bloomRPC" src="https://user-images.githubusercontent.com/22433243/127911346-42ec13c0-6947-4888-926b-1bb9b9bb58c4.png">

### Locally

![Server](https://user-images.githubusercontent.com/22433243/127906948-3aeb3316-6a7a-4f9f-ad0b-b790c5f54ad5.png)

![Client](https://user-images.githubusercontent.com/22433243/127906965-71872380-4d42-495a-90b0-1c0ca431e1a7.png)
