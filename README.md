# localhost-services

一个用于本地开发的轻量服务集合（Docker Compose 配置），包含 PostgreSQL、Redis 等常用服务。

快速开始
- 克隆仓库到本地。
- 在仓库根目录运行：

```
docker-compose up -d
```

数据目录
- 本地卷和数据保存在 `data/` 下（包括 `postgres/`、`redis/` 等），便于备份与恢复。

说明
- 本仓库用于在本地快速搭建依赖服务，不包含应用代码。根据需要可修改 `docker-compose.yml` 的服务配置。

维护者: 仓库所有者
