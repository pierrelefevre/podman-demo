## Install podman
sudo dnf install podman

## Containers
podman build hello-devops --tag devops:nginx

podman run -p 8082:8080 devops:nginx

**Check your browser at localhost:8082**

## Compose
podman-compose up -d --build

## View running containers
podman ps

## Attach to a running container
podman exec -it CONTAINER-ID /bin/bash

*Ricky!*

**Check your browser at localhost:8081**

## K8s resources
**Show the deployment.yaml**

podman play kube deployment.yaml

**Check your browser at localhost:8080**

## Comparing desktop GUI offerings

**Open podman desktop and docker desktop**

show the similar gui and compare with docker desktop

- podman has a "Pod" tab that has a Pod in it from the *deployment.yaml*

## Podman in Github Actions

show .github/workflows/build-and-push.yml

then do: **git push**, and see the result of the GitHub action in in Github.com
