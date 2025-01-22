# MobaXterm-GenKey
你懂的！！

## 演示地址
http://192.99.11.204:5000/



## 本地启动
需要安装Python3!!!
```
pip install --no-cache-dir -r requirements.txt
python app.py
```

## Docker
```
docker pull malaohu/mobaxterm-genkey
docker run -d -p 5000:5000 malaohu/mobaxterm-genkey
```

## docker-compse

malaohu/mobaxterm-genkey 是不支持arm的，需要自行打包镜像

```
下载代码，进入对应的目录
docker build -t malaohu/mobaxterm-genkey:3.6 .
```

使用docker-compose来启动镜像
```
version: '3'

services:
  mobaxterm-genkey:
    image: malaohu/mobaxterm-genkey:3.6
    container_name: mobaxterm-genkey
    restart: unless-stopped
    ports:
      - "5000:5000"
```


## 使用方法
访问：IP:5000
![image](https://user-images.githubusercontent.com/8140841/116803404-e94c8300-ab49-11eb-83db-ad0246ebedd3.png)

### 激活方式
直接放到软件目录即可！



核心内容来自：https://github.com/flygon2018/MobaXterm-keygen
详细介绍文章：https://51.ruyo.net/17008.html
