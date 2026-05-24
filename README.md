# 汇总知识点

## MySQL

## Vue23

## TypeScript

## Redis

## Docker

### 启动一个docker服务并挂载目录
```
docker run -d \
  --name nginx \
  --network=host \
  --restart=always \
  -v /root/docker/nginx/conf/conf.d:/etc/nginx/conf.d \
  -v /root/docker/nginx/ssl:/etc/nginx/ssl \
  -v /root/docker/nginx/html:/usr/share/nginx/html \
  nginx
```

## Linux

### 上传文件或目录
```
scp -r idiom.cn.key username@IP:/root/docker/nginx/ssl
```