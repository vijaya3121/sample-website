# 🌐 Sample Website - Docker Packaging

This repository contains a simple HTML website which is packaged as a Docker container using **Nginx**.

---

## 🔧 Dockerfile

```Dockerfile
FROM nginx:latest
COPY index.html /usr/share/nginx/html/index.html
```
## 🧱 Build Docker Image
```
docker build -t sampleweb:v1 .
```
## ▶️ Run the Container
```
docker run -d -p 8080:80 --name samplewebapp sampleweb:v1
```
## 🌍 Test in Browser
```
http://<your_vm_public_ip>:8080
```
## 📸 Proof (Screenshots)
### Docker Build Success:
![docker build](https://github.com/vijaya3121/sample-website/blob/main/docker%20build.png)

### Docker Run Output:
![docker run with port 8080](https://github.com/vijaya3121/sample-website/blob/main/docker%20port.png)

### Browser Output:
![Browser output](https://github.com/vijaya3121/sample-website/blob/main/browser%20output.png)
