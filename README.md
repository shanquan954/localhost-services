# localhost-services

一个用于本地开发的轻量服务集合（Docker Compose 配置），包含 PostgreSQL、Redis、MySQL 等常用服务。

快速开始
- 克隆仓库到本地。
- 复制 `env.example` 为 `.env` 并按需修改变量（默认密码均为 `shanquan`）。
- 在仓库根目录运行：

```
docker-compose up -d
```

数据目录
- 本地卷和数据保存在 `data/` 下（包括 `postgres/`、`redis/`、`mysql/` 等），便于备份与恢复。

环境变量
- `.env` 由 `env.example` 拷贝，包含 PostgreSQL、Redis、MySQL 所需配置。
- MySQL 依赖 `MYSQL_ROOT_PASSWORD`、`MYSQL_DATABASE`、`MYSQL_USER`、`MYSQL_PASSWORD`、`MYSQL_PORT`，默认示例均为 `shanquan`，端口默认 3306。

说明
- 本仓库用于在本地快速搭建依赖服务，不包含应用代码。根据需要可修改 `docker-compose.yml` 的服务配置。

维护者: 仓库所有者
