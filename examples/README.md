# Pumba Demo

## Stop/Restart random container

1. Split screen horizontally
1. Run 10 Docker containers in bottom screen: `./stop_demo.sh`
1. Run `pumba` stopping and restarting random container: `./pumba_stop.sh`

## Pause/Resume Docker container

1. Split screen horizontally
1. Run test container printing time every second: `./pause_demo.sh`
1. Run `pumba` to pause/resume main process: `./pumba_pause.sh`

## Delay network traffic

1. Split screen horizontally
1. Run "ping" container pinging `1.1.1.1`: `./delay_demo.sh`
1. Run `pumba` adding `3000ms ± 20` delay to the "ping" container: `./pumba_delay.sh`

## Add packet loss to egress traffic

1. Split screen horizontally
1. Split bottom screen vertically
1. On the right bottom screen run UDP server: `./loss_demo_server.sh`
1. On the left bottom screen run UDP client: `./loss_demo_client.sh`; send datagrams to the UDP server
1. Run `pumba` adding packet loss to client egress traffic: `./pumba_loss.sh`

## Stress-testing container

1. Split screen horizontally
2. Run test container and show Docker stats: `./stress_demo.sh`