# gRPC

###For generate pb.go
``` protoc *.proto \
    --go_out=. \
    --go_opt=paths=source_relative \
    --proto_path=. 
```

###Also we need 
```
$ brew install grpc 
$ go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.26
```