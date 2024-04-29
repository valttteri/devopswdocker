### I completed the exercise with this single command

```bash
docker run --rm -it --name search ubuntu sh -c "apt-get update && apt-get install -y curl && while true; do echo 'Input website:'; read website; echo 'Searching..'; sleep 1; curl http://$website; done;"
```
