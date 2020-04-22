# docker-compose 部署 acme.sh申请Let's encrypt 证书

> acme.sh 实现了 acme 协议, 可以从 letsencrypt 生成免费的证书.

 > [acme.sh地址](https://github.com/acmesh-official/acme.sh/wiki/Run-acme.sh-in-docker)
 
 > [获取阿里云AccessKey](https://usercenter.console.aliyun.com/?spm=5176.12818093.nav-right.dak.488716d0qgnmuw#/manage/ak)
 
```bash
# 编辑docker-compose.yml填入阿里云获取的key

# 启动容器
docker-compose.yml up -d

# 生成证书 (生成证书放在当前目录ssl)
docker exec acme.sh \
    --issue \
    --dns dns_ali \
    -d '*.hackshen.com' 
```
