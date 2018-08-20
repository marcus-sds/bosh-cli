# bosh-cli

## Requirements

- Go

https://medium.com/@patdhlk/how-to-install-go-1-9-1-on-ubuntu-16-04-ee64c073cd79

- direnv

https://github.com/direnv/direnv/releases


## compile

1. download bosh cli

1. .envrc configuration

	export PATH=/usr/local/go/bin:$PATH
	export GOPATH=$PWD

1. change source and build

	vi ./src/github.com/cloudfoundry/bosh-cli/vendor/github.com/cloudfoundry/config-server/types/certificate_generator.go
	cd $GOPATH/src/github.com/cloudfoundry/bosh-cli
	./bin/build
	cd out; ./bosh --version
