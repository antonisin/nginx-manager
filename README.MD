# Nginx Proxy Manager - Docker
[![img](https://img.shields.io/badge/-docker-blue?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)


## Author
Maxim Antonisin <br>
[![img](https://img.shields.io/badge/-maxim.antonisin%40gmail.com-blue?style=for-the-badge&logo=gmail)](mailto:maxim.antonisin@gmail.com) <br>
[![img](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mantonishin/)

Original (Reference and original repository) <br>
[![img](https://img.shields.io/badge/-github-blue?style=for-the-badge&logo=github)](https://github.com/NginxProxyManager/nginx-proxy-manager)


## Description
This repository provides easy-to-use Docker Compose configuration files for deploying and managing Nginx Proxy Manager.
Nginx Proxy Manager is a powerful tool for routing and securing web traffic, and this repository simplifies the process
of deploying it on a local machine or server. With these files, you can quickly and easily set up a robust proxy
management solution that streamlines your web development workflow. This repository is based on the original source code
from the NginxProxyManager/nginx-proxy-manager repository.

**Thank you to the authors for creating this useful tool, and I hope this repository helps others make the most of it.**

## Requirements
[![img](https://img.shields.io/badge/-docker-blue?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![img](https://img.shields.io/badge/-docker--compose-blue?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)

## Use

### Run
```bash
docker-compose up
```
or detached mode
```bash
docker-compose up -d
```

### Stop
```bash
docker-compose down
```

### URL
```
http://localhost:81
```
or
```
http://[IP]:81
```

### Notes
When configuring a host proxy in a Docker container, consider using the container's name instead of its IP address. The
container's name is static and won't change, unlike its IP address, which can change when the container is restarted or
recreated. Simply replace the container's IP address with its name in your proxy configuration file to make it more
resilient to changes.