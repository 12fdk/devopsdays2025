---
title: K8S
---
![k8s](k8s.svg.png)

Docker is fine, but let's try the K8s as well

Let's start by opening K9S, which is included in the image.

```execute-1
k9s
```

```execute-2
kubectl run nginx-demo --image=bitnami/nginx:latest --port=8080   --overrides='{"spec":{"securityContext":{"runAsNonRoot":true},"containers":[{"name":"nginx-demo","image":"bitnami/nginx:latest","ports":[{"containerPort":8080}],"securityContext":{"allowPrivilegeEscalation":false,"capabilities":{"drop":["ALL"]},"runAsNonRoot":true}}]}}'
```

