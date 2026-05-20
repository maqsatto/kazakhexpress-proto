# KazakhExpress Proto

Shared protobuf contracts and generated Go clients/servers for KazakhExpress microservices.

## Layout

```txt
proto/kazakhexpress/payment/v1/payment.proto
proto/kazakhexpress/smtp/v1/smtp.proto
gen/go/... generated Go code
```

## Generate

```powershell
go install github.com/bufbuild/buf/cmd/buf@latest
go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest
buf generate
go test ./...
```

## Use From Services

```powershell
go get github.com/maqsatto/kazakhexpress-proto
```
