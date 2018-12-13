项目github地址如下
https://github.com/BigBrother3

本篇文档主要是展示一下项目中的api

# 查找资源api
直接用get请求 http://localhost:8080/api/films/1 ，就可以得到资源。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20181213125532875.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0REZ2hzb3Q=,size_16,color_FFFFFF,t_70)
资源的api主要有

总的api，默认返回第一页的内容，每页有5个资源
```
http://localhost:8080/api/films
http://localhost:8080/api/people
http://localhost:8080/api/planets
http://localhost:8080/api/species
http://localhost:8080/api/starships
http://localhost:8080/api/vehicles
```

按页搜索的api，每页有5个资源
``` 
http://localhost:8080/api/films/?pages=%d
http://localhost:8080/api/people/?pages=%d
http://localhost:8080/api/planets/?pages=%d
http://localhost:8080/api/species/?pages=%d
http://localhost:8080/api/starships/?pages=%d
http://localhost:8080/api/vehicles/?pages=%d
```
 
按个搜索的api
```
http://localhost:8080/api/films/%d
http://localhost:8080/api/people/%d
http://localhost:8080/api/planets/%d
http://localhost:8080/api/species/%d
http://localhost:8080/api/starships/%d
http://localhost:8080/api/vehicles/%d
```

# 注册用户api
向http://localhost:8080/register 发送post请求，并将用户名和密码的信息发出，就可以看到服务端返回成功的字样。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20181213125632418.jpg)

# 登陆用户api
向http://localhost:8080/login 发送post请求，并将之前注册的用户名和密码发出，可以看到服务器传回来一个token，通过这个toke就可以验证用户是否登陆了。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20181213125828267.jpg)
