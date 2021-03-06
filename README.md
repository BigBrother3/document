# 项目文档
本项目模仿 https://swapi.co/ 实现SWAPI相关的功能，添加了资源的授权访问部分的内容

## 前后端安装说明
1. 前端使用Vue框架搭建
``` bash
# 安装Vue命令行工具
npm install --global vue-cli

# 安装一个新项目（此步骤省略）
npm install -g @vue/cli-init
vue init webpack my-project

# 安装依赖
cd 项目所在的文件夹（如：swapi/）
npm install

# 服务以热重载的方式运行在 localhost:8000
npm run dev

# 可能需要安装的依赖
npm install vue-cookies --save // cookies服务
npm install vue-resource --save // http服务
```

2. 后端使用Go语言实现,运行在localhost:8080，使用如下命令安装
```
go get github.com/BigBrother3/server
```
##  Overview
客户端代码仓库：https://github.com/BigBrother3/client

服务端代码仓库：https://github.com/BigBrother3/server

1. 页面(3个)  
登陆、注册、查询页
2. 资源类型(6个)  
films、people、planets、species、starships、vehicles
3. 数据来源  
资源数据均抓取与源网站 https://swapi.co/ 
4. 授权访问采用jwt验证
5. 服务api  
获取资源目录(受限资源)  
/api/ GET  
films资源  
/api/films/?page={id} GET  
/api/films/pages GET  
/api/films/{id} GET  
people资源  
/api/people/?page={id} GET  
/api/people/pages GET  
/api/people/{id} GET  
planets资源  
/api/planets/?page={id} GET  
/api/planets/pages GET  
/api/planets/{id} GET  
species资源  
/api/species/?page={id} GET  
/api/species/pages GET  
/api/species/{id} GET  
starships资源  
/api/starships/?page={id} GET  
/api/starships/pages GET  
/api/starships/{id} GET  
vehicles资源  
/api/vehicles/?page={id} GET  
/api/vehicles/pages GET  
/api/vehicles/{id} GET  
注册登陆  
/register POST(username&password)  
/login POST(username&password)