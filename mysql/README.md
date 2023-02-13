# mysql部署文档

## 1.部署容器

### 1.1 将当前`mysql`目录拷贝上传至需要部署的服务器，并进入

```
cd mysql
```

### 1.2 启动容器

```
docker-compose up -d
```

## 2.配置mysql（可选操作）

### 2.1 自定义配置

```
将mysql的"xxx.cnf"配置文件拷贝到启动容器后生成的"conf"目录下，重启容器即可完成配置。
```

### 2.2 初始化数据库

```
先将mysql的"xxx.sql"初始化文件拷贝到"init"目录下，再启动容器即可完成初始化（注意：对于同一个容器，初始化sql只会生效一次）。
```