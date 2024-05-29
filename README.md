# Install raspberry pi

## Preparation

1. Install image (https://www.raspberrypi.com/software/)
2. Secure raspberry pi - ssh only via key (https://janw.me/raspberry-pi/only-allow-ssh-key-login-on-raspberry-pi/)
3. Install docker `curl -sSL https://get.docker.com | sh`
4. Start and setup portainer: 
   1. Run `sudo docker run -d -p 9000:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer-ce:latest`. This starts the portainer container and restarts it on ever boot.
   2. Setup a stack and add the raspberrypi repo.