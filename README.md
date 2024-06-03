# Docker
How to Install docker &amp; portainer in your Ubuntu System.

## Step 1: Install Docker on Ubuntu

1. Update the package list:

   ```shell
   sudo apt-get update
   ```
2. Install Docker:

   ```shell
   sudo apt-get install docker.io
   ```
3. Check the docker version:

   ```shell
   sudo docker --version
   ```
   
4. You can start the Docker service and configure it to run on startup by entering the following commands:

   ```shell
   sudo systemctl start docker
   sudo systemctl enable docker
   ```
5. Verify the status of the docker service:

   ```shell
   systemctl status docker
   ```

## Step 2: Install Portainer on Ubuntu

1. Run the following command to pull the Portainer image from Docker Hub:

   ```shell
   docker pull portainer/portainer-ce:latest
   ```
2. Run Portainer:

   ```shell
   docker run -d -p 9000:9000 --restart always -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer-ce:latest
   ```
3. Access Portainer:

   ```shell
   Open a web browser and navigate to http://localhost:9000
   ```
