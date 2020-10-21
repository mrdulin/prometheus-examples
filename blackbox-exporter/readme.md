# blackbox exporter

启动 exporter 和 prometheus

```bash
docker-compose up
```

http://localhost:9115 查看 exporter 控制台页面

http://localhost:9115/metrics 包含 exporter 自身的指标，以便同时监控 exporter 本身

- 查看 http_2xx_check 指标: http://localhost:9115/probe?target=www.example.com&module=http_2xx_check
- 查看 icmp_check 指标: http://localhost:9115/probe?target=prometheus.io&module=icmp_check
- 查看 dns_examplecom_check 指标:

开启 debug 信息: http://localhost:9115/probe?target=prometheus.io&module=http_2xx_check&debug=true
