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

