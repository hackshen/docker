# docker
> 部署一些日常使用的环境
> 现有环境: Nginx、 acme.sh、 Frp


#### Install docker
- [https://docs.docker.com/install/linux/docker-ce/centos/](https://docs.docker.com/install/linux/docker-ce/centos/)

#### Install docker-compose
```bash
# install
sudo curl -L https://get.daocloud.io/docker/compose/releases/download/1.25.4/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose

# Add permissions
sudo chmod +x /usr/local/bin/docker-compose
```
