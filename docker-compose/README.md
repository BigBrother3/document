# Docker实验报告

1. [Docker概念](##Docker概念)
2. [使用MYSQL数据库](#SQL数据库)
3. [SWAPI容器化](#SWAPI容器化)

## Docker概念
Docker 是一种用来快速部署服务的容器技术。Docker提供简单易用的容器使用接口。它是目前最流行的 Linux 容器解决方案。Docker 将应用程序与该程序的依赖，打包在一个文件里面。运行这个文件，就会生成一个虚拟容器。程序在这个虚拟容器里运行，就好像在真实的物理机上运行一样。使用Docker,使得部署应用时不用担心环境问题。更快速的交付和部署，高效的部署和扩容，更高的资源利用率，更简单的管理。

## SQL数据库
SWAPI应用中数据库改为使用MYSQL
代码地址：https://github.com/BigBrother3/server/tree/dockerServer/database

## SWAPI容器化
容器dockerfile和stack.yml文件地址：https://github.com/BigBrother3/document/tree/master/docker-compose