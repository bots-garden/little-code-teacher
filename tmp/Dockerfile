FROM node:21-bookworm
ARG OLLAMA_BASE_URL
ENV OLLAMA_BASE_URL=${OLLAMA_BASE_URL}
USER node
RUN mkdir -p /home/node/app
WORKDIR /home/node/app
COPY --chown=node . .
RUN yarn install
CMD ["yarn", "start"]



