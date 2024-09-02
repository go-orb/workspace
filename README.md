# go-orb workspace

This is our workspace to easily develop go-orb, it contains [go-orb](https://github.com/go-orb/go-orb) it's [plugins](https://github.com/go-orb/plugins) and [examples](https://github.com/go-orb/examples).

We use `go.work` for development and [task](https://taskfile.dev/) to execute common tasks.

## Install

Clone the repo:

```sh
git clone --recurse-submodules -j8 git@github.com:go-org/workspace.git
```

Install task:

```sh
go install github.com/go-task/task/v3/cmd/task@latest
```

## License

go-orb is Apache 2.0 licensed and is based on go-micro.