# proto
Wrapper around proto-c releases for building with go modules.  Copies the google well know type includes to mod directory.  Intent is to track upstream changes and versions with matched tags.

## usage
When building protos, include the directory that this pulls in the protoc command.

## example with vendors
```sh
protoc --gogoslick_out=Mgoogle/protobuf/any.proto --proto_path=. --proto_path=./vendor/ProfessorMc/proto/. protofile.proto
```
## example on gopath
```sh
protoc --gogoslick_out=Mgoogle/protobuf/any.proto --proto_path=. --proto_path=$(GOPATH)/github.com/ProfessorMc/proto/. protofile.proto

```


