# frp

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
