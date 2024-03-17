# little-code-teacher

```bash
docker build -t little-code-teacher .

docker run -d -p 6060:8080 --name little-code-teacher-prod -e "OLLAMA_BASE_URL=https://ollama-malin-bots-garden.koyeb.app/" --rm little-code-teacher
```


