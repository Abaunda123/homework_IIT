# Static Website Docker Image

This is a static HTML website containerized for the **DevOps with Docker** course (Exercise 1.15). 
The site is served using a lightweight **Nginx** server on Alpine Linux.

## Description

This repository contains:
- A static web page (`index.html` and assets).
- A `Dockerfile` that packages the site into an Nginx-based container.
- Automated deployment instructions.

## How to build the image

First, clone the repository to your local machine, then run:

docker build -t html-site .

## How to run the container

docker run -p 8080:80 html-site

Then open your browser at:

http://localhost:8080

## Docker Hub

# Pull the image
docker pull abaunda123/html-site

# Run the container
docker run -p 8080:80 abaunda123/html-site