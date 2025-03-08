# go-orb workspace

This is our workspace to easily develop go-orb, it contains [go-orb](https://github.com/go-orb/go-orb) it's [plugins](https://github.com/go-orb/plugins) and [examples](https://github.com/go-orb/examples).

We use `go.work` for development.

## Install

Clone the repo:

```sh
git clone --recurse-submodules -j8 https://github.com/go-orb/workspace.git go-orb
```
## Development

You need:
- go1.23.6 or later
- docker for dagger
- our custom fork of [wire](https://github.com/go-orb/wire) `go install github.com/go-orb/wire/cmd/wire@latest`
- [protoc-gen-go](https://protobuf.dev/reference/go/go-generated/) `go install google.golang.org/protobuf/cmd/protoc-gen-go@latest`
- [protoc-gen-go-orb](https://github.com/go-orb/plugins/server/cmd/protoc-gen-go-orb) `go install github.com/go-orb/plugins/server/cmd/protoc-gen-go-orb@latest`

Now you'r able to run `go generate ./...` in the examples to update `cmd/xyz/wire_gen.go` as well as the `proto` files.

## License

go-orb is Apache 2.0 licensed and is based on go-micro.