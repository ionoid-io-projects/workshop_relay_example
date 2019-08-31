# Introduction
Making led blink 

# How to
Compile relay.go like this
```
go get github.com/stianeikeland/go-rpio
env GOOS=linux GOARCH=arm GOARM=6 go build relay.go
```
Copy the generated file to your raspberry pi device and execute it with this command

```
env RPIO_PIN=21 BLINK_INTERVAL=1 ./relay
```

# env variables used
RPIO_PIN = an integer to define rpi pin used in wiring, default 21
BLINK_INTERVAL = time interval in second, default 1

Happy blinking 