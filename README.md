# 通过Grafana+Prometheus+redis-streams-exporter，监控redis streams

## 1.快速使用
```
$ cd redis-streams-monitoring                       # 进入项目目录
$ cp env.sample .env                                # 复制环境变量文件
$ cp docker-compose.sample.yml docker-compose.yml   # 复制 docker-compose 配置文件。
$ docker-compose up                                 # 启动
```
## 2.访问
1. Grafana http://127.0.0.1:3000 [admin:admin]
2. Prometheus http://localhost:9090/targets

## 3.在Grafana增加Prometheus数据源
1. 添加数据源
2. 进入后搜索关键字 `redis`
3. 使用`grafana/dashboards.json`
4. 看吧😁

## 4.开源地址
1. https://github.com/grafana/grafana
2. https://github.com/prometheus/prometheus
3. https://github.com/chrnola/redis-streams-exporter