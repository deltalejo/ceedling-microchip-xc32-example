# Ceedling Microchip XC32 Example

Sample project illustrating the setup and usage of Microchip's XC32 compiler and
Ceedling along with the [MDB plugin](https://github.com/deltalejo/ceedling-mdb-plugin)
for running tests both on simulator and target.

## Try this out

Clone:

```shell
git clone --recurse-submodules https://github.com/deltalejo/ceedling-microchip-xc32-example.git
```

Run tests on simulator:

```shell
ceedling test:all
```

Run tests on target:

```shell
ceedling mdb:hwtool[<debugger>] mdb:serialport[<port>] test:all
```

E.g.:

```shell
ceedling mdb:hwtool[snap] mdb:serialport[/dev/ttyUSB0] test:all
```
