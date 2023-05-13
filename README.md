# frp

https://github.com/fatedier/frp

### Docker

Start the Server:
```bash
docker-compose -f docker-compose-server.yml up
```

Start the Client:
```bash
docker-compose -f docker-compose-client.yml up
```

### Kubernetes

Deploy the Server:
```bash
kubectl apply -f k8s/server
```

Deploy the Client:
```bash
kubectl apply -f k8s/client
```

Create a nginx pod and expose it:
```bash
kubectl run nginx --image nginx:alpine
kubectl expose pod nginx --port 80
```

### Kubeconfig

Test your private cluster:
```bash
kubectl --insecure-skip-tls-verify get pods
```

### SSH

SSH into the server:
```bash
ssh ubuntu@k8s.shubhamtatvamasi.com

# custom port
ssh ubuntu@k8s.shubhamtatvamasi.com -p 2222
```
