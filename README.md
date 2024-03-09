# little-code-teacher


docker build -t little-code-teacher .

docker run -d -p 6060:8080 --name little-code-teacher-prod -e "OLLAMA_BASE_URL=https://ollama-malin-bots-garden.koyeb.app/" --rm little-code-teacher



#!/bin/bash
IMAGE_BASE_NAME="little-code-teacher"
IMAGE_TAG="0.0.0"
docker login -u ${DOCKER_USER} -p ${DOCKER_PWD}
docker buildx build --platform linux/amd64 --push -t ${DOCKER_USER}/${IMAGE_BASE_NAME}:${IMAGE_TAG} .

