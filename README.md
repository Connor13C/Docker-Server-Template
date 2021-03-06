# Server

This is the server side setup and configuration to host multiple applications through an
nginx reverse proxy server. All setup is in docker-compose.yml. Non-image docker setups have a Dockerfile in the related folder.

To run:
* Install Docker - choices:
   * [From documents](https://docs.docker.com/install/)
   * [From bash script](https://get.docker.com)
* Change proxy/default.conf file lines 16, 28, 40, 49, 56, & 65 to your own website setup
* Change proxy/website.csr to contain your website csr
* Change proxy/website.key to contain your private key
* Change proxy/website.pem to contain your website certificate chain
* Run Containers:
   * sudo docker-compose up -d
* Stop Containers:
   * sudo docker-compose down
* List Volumes:
   * sudo docker volume ls
