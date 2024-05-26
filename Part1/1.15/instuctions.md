## Exercise 1.15 instructions

Link to the image on [Docker Hub](https://hub.docker.com/layers/valtteri1/devopswdocker1/latest/images/sha256-beb6dc74b431b106753974a1b94c5d926ee6117f4b19d4ef42399d25eb4542ba?tab=layers) \
Link to the project [repository](https://github.com/valttteri/simple_web_app)

Pull the image from Docker Hub  
```docker pull valtteri1/devopswdocker1```

Start a container \
```docker run -p 8000:8000 valtteri1/devopswdocker1```

The application will start running in a browser at http://localhost:8000. It is a simple phonebook app where you can add new contacts and remove them.
