### Lib protocol buffer
go get -u google.golang.org/grpc  
go get -u github.com/golang/protobuf/protoc-gen-go  

### Generate proto file
protoc --proto_path=proto proto/*.proto --go_out=plugins=grpc:pb  

### Create Makefile