# WireGuardDocker
Docker container Wireguard VPN server
<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/98/Logo_of_WireGuard.svg/2560px-Logo_of_WireGuard.svg.png" width="500" title="logo">
</p>
<p align="center">
  <img src="https://www.docker.com/sites/default/files/d8/2019-07/horizontal-logo-monochromatic-white.png" width="500" title="logo">
</p>


### Config.
- Change the value of variable `PEERS=3` to the desired number of customers.
- Open the UDP 51820 port on the router, and point it to the IP of the server where you are running the container. 

### Launch
`docker-compose -up d`

### View logs
`docker logs wireguard`

### Monitor traffic from a connected client,
- Access to the container: `docker exec -it wireguard bash` 
- And once inside, we execute: `wg show`
