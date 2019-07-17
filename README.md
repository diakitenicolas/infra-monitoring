# infra
Infra 

## Requirement

* If not exists , create `traefik` network before
```
docker network create traefik
```


* Create User for prometheus/alermanager Dashboard 
```
htpasswd -nb monitor changeme

```

Add an entry in your env vas like
 `MONITOR_BASICAUTH=monitor:$apr1$Lscox9Mm$EsK/hzJsNNDBGf68vUHV6/` where `monitor:$apr1$Lscox9Mm$EsK/hzJsNNDBGf68vUHV6/` is the result of your htpasswd.

 
* For grafana it is admin/changeme123
