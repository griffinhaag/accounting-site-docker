# Accounting Site: Dockerized

A DevOps class exercise in containerizing a static website. The site is Colorlib's free "Accounting" Bootstrap 4 template. My part was packaging it with Docker, serving it with Apache, and publishing the image to Docker Hub.

## Files

```
Dockerfile           Copies the site into an Apache httpd 2.4 image
docker-compose.yml   Runs the published image (griffinh00/accountingweb) on port 80
*.html, css/, js/    The template
```

## Running it

```bash
docker compose up
```

Then open http://localhost.

Or build it yourself:

```bash
docker build -t accountingweb .
docker run -p 8080:80 accountingweb
```
