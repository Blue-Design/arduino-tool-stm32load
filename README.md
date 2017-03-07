# arduinoSTM32load
multiplatform launcher for [Arduino STM32F4 Core](https://github.com/arduino-org/arduino-core-stm32f4) dfu-util flashing utility

## Compiling

* Download go package from [here](https://golang.org/dl/) or using your package manager
* `cd` into the root folder of this project
* execute
```bash
export GOPATH=$PWD
export GOBIN=.
go get -d
go build
```
to produce a binary of `arduinoSTM32load` for your architecture.

To cross compile for different OS/architecture combinations, execute
```bash
GOOS=windows GOARCH=386 go build  #windows
GOOS=darwin GOARCH=amd64 go build #osx
GOOS=linux GOARCH=386 go build    #linux_x86
GOOS=linux GOARCH=amd64 go build  #linux_x86-64
```
## Credits
`arduinoSTM32load` is based on [arduino101load](https://github.com/facchinm/arduino101load) by [Martino Facchin](https://github.com/facchinm)
