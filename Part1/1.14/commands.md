### Backend commands

```
docker build . -t back
docker run -p 127.0.0.1:8080:8080 back
```

### Frontend commands

```
docker build . -t front
docker run -p 127.0.0.1:5000:5000 front
```