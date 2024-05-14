## ARL(Asset Reconnaissance Lighthouse)资产侦察灯塔系统
原有Readme已备份， 请移步至 Readme-Old <br>
[ARL官方仓库](https://github.com/TophantTechnology/ARL) https://github.com/TophantTechnology/ARL
该版本Fork时间为7个月之前

### 运行方法
docker-compose安装（曾经的官方推荐）
```
    cd /opt/
    mkdir docker_arl
    wget -O docker_arl/docker.zip https://github.com/PawsProjects/ARL/releases/download/Release/DockerBackup.zip
    cd docker_arl
    unzip -o DockerBackup.zip
    docker-compose pull
    docker volume create arl_db
    docker-compose up -d
```
本docker镜像备份于七月前，可能过时或者含有已知漏洞

---
从源码安装
```
wget https://raw.githubusercontent.com/PawsProjects/ARL/master/misc/setup-arl.sh
chmod +x setup-arl.sh
./setup-arl.sh
```
### 目标

- [x] 修复构建文件依赖，可以使用源码构建
- [x] 重建Docker镜像，可以直接通过docker-compose部署
- [ ] 增加对IP资产的支持
