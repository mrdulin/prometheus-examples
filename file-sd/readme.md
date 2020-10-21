# USE FILE-BASED SERVICE DISCOVERY TO DISCOVER SCRAPE TARGETS

```bash
prometheus-2.22.0.darwin-amd64  ./prometheus --config.file=/Users/ldu020/workspace/github.com/mrdulin/prometheus-examples/file-sd/prometheus.yml
```

访问 http://localhost:9090/service-discovery, 通过 Web 界面查看服务发现目标的完整列表及其元数据标签。

### Reference

- https://prometheus.io/docs/guides/file-sd/
