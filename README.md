# gRPC

### For generate pb.go

``` 
protoc *.proto \
    --go_out=. \
    --go-grpc_out=. --go-grpc_opt=paths=source_relative \
    --go_opt=paths=source_relative \
    --proto_path=. 
```

### Also we need

```
$ brew install grpc 
$ go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.26
```

```
export PATH="$PATH:$(go env GOPATH)/bin"
```
