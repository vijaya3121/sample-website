# 🌐 Sample Website - Docker Packaging

This repository contains a simple static HTML website which is containerized using **Docker** and served using **Nginx**.  
The purpose of this project is to demonstrate how a basic web page can be packaged and deployed as a Docker container.

---

## 📂 Repository Structure
| File | Purpose |
|------|---------|
| index.html | Sample website homepage |
| Dockerfile | Instructions to build Nginx-based image |

---

## 🔧 Dockerfile

```Dockerfile
FROM nginx:latest
COPY index.html /usr/share/nginx/html/index.html
```
---

## 🧱 Build Docker Image
```
docker build -t sampleweb:v1 .
```
---
## ▶️ Run the Container
```
docker run -d -p 8080:80 --name samplewebapp sampleweb:v1
```
---
## 🐳 Running Containers Check
```
docker ps
```
---
## 🌍 Test in Browser
```
http://<your_vm_public_ip>:8080
```
---
## 📸 Proof (Screenshots)
### Docker Build Success:
![docker build](https://github.com/vijaya3121/sample-website/blob/main/docker%20build.png)

### Docker Run Output:
![docker run with port 8080](https://github.com/vijaya3121/sample-website/blob/main/docker%20port.png)

### Browser Output:
![Browser output](https://github.com/vijaya3121/sample-website/blob/main/browser%20output.png)

---
## Future Enhancements
- Deploy to Kubernetes
- Push image to Azure Container Registry (ACR)
- Automate builds using GitHub Actions CI/CD
---
## 👩‍💻 Author

Vijaya Reddy
DevOps & Cloud Enthusiast
