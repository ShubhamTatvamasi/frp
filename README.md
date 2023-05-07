# frp

https://github.com/fatedier/frp

### Docker

Start the server:
```bash
docker-compose -f docker-compose-server.yml up
```

Start the client:
```bash
docker-compose -f docker-compose-client.yml up
```

### Kubernetes

Deploy the Server:
```bash
kubectl apply -f k8s
```

Test your private cluster:
```bash
kubectl --insecure-skip-tls-verify get pods
```

### SSH

SSH into the server:
```bash
ssh ubuntu@k8s.shubhamtatvamasi.com -p 2222
```
