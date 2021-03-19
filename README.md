```bash
helm install --name squid .
kubectl port-forward -n default service/squid 3128:3128
http_proxy="http://holosix:xN186VaYjrCGepJI@localhost:3128" https_proxy="http://holosix:xN186VaYjrCGepJI@localhost:3128" curl  ipinfo.io/ip
```

