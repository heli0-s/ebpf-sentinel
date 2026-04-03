# ebpf-sentinel

**10分钟部署的容器运行时威胁检测 · 比 Falco 简单10倍 · 零误报设计**
```bash
kubectl apply -f https://raw.githubusercontent.com/你/ebpf-sentinel/main/deploy/daemonset.yaml
```

部署完成后，当容器内出现反弹 shell、异常外联、特权逃逸时，
你的 Slack 会在 3 秒内收到告警。

[截图：Slack告警消息]

## 为什么不用 Falco

| | Falco | ebpf-sentinel |
|---|---|---|
| 部署时间 | 2天调规则 | 10分钟 |
| 误报率 | 高（需要持续调优） | 低（5条精准规则） |
| 资源占用 | 高 | < 1% CPU |
| 价格 | $50,000/年（企业版） | $199/月/集群 |

## 快速开始
...
