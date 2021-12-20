# Proglog

Github Repository for following along with the 'Distributed Services with Go' book by Travis Jeffery.

## Installing and using the Go protobuf runtime

_Compilation is within [Makefile](./Makefile)_.

```go get google.golang.org/protobuf/...@v1.27.1``` - https://pkg.go.dev/google.golang.org/protobuf

```sh
protoc api/v1/*.proto \
  --go_out=. \
  --go_opt=paths=source_relative \
  --proto_path=.
```