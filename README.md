# 🚧 Coming Soon Page (Nginx + Kubernetes)

This project provides a lightweight, animated "Coming Soon" page built using HTML, CSS, and JavaScript, served by an NGINX container in a Kubernetes cluster. It’s ideal as a placeholder while your main application is in development or deployment.

**Demo:** [https://amidmast.github.io/coming-soon/](https://amidmast.github.io/coming-soon/)

## ✨ Features

- Clean and responsive UI with animated header
- Dynamic IP and User-Agent display using NGINX variables
- Clipboard copy functionality for request ID
- Real-time year display
- Toast notifications for user feedback
- No caching or search engine indexing (SEO disabled)
- Dockerized for easy deployment
- Kubernetes-ready with minimal resource usage

## 📁 File Structure

- `index.html` – Main "Coming Soon" webpage
- `favicon.png` – Custom favicon
- `nginx.conf` – NGINX configuration with a custom `/ip/info` endpoint
- `Dockerfile` – Docker image build instructions
- `coming-soon.yaml` – Kubernetes manifest for deployment and service

## 🐳 Docker

To build and run the container locally:

```bash
docker build -t coming-soon .
docker run -p 8080:80 coming-soon

