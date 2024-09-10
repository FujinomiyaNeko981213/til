# redash部署坑

1. Redash创建的时候要初始化数据库 
```bash
docker-compose run --rm server create_db

```

2. Redash构建镜像时，skip_frontend_build不知道为什么默认传递了true导致前端没有构建（环境 MacBook Pro Intel）