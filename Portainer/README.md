
## Installation of  Portainer on Ubuntu 22.04

1. Run the following command to pull the Portainer image from Docker Hub:

   ```shell
   docker pull portainer/portainer-ce:latest
   ```
2. Run Portainer:

   ```shell
   sudo docker run -d -p 9000:9000 --restart always -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer-ce:latest
   ```
3. Access Portainer:

   ```shell
   Open a web browser and navigate to http://YOUR_IP_ADDRESS:9000
   ```