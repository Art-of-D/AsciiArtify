# Steps to Run ArgoCD

---

To start k3d cluster with Argo CD follow the video
![](argocd.gif)

---

Generate password when you forward port after kubectl port-forward svc/argocd-server -n argocd 8080:443:

open other terminal window and use

```
k -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}"
  cFZIWTM3eFpJR3hDeUxLNQ==# <--- you will get pass in base64
k -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}"|base64 -d;echo
  pVHY37xZIGxCyLK5 <--- you will get your pass
```

---

1. Go to http://localhost:8080
2. Log in

- Default username: admin
- password: from previous step

3. Then follow the next video

https://github.com/Art-of-D/AsciiArtify/assets/114071335/d786affc-a64e-478a-a065-f2a3c82058da

