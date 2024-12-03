### Build Your Docker Image
```docker
    docker build -t my-docker-app .
```

### Run Your Docker Container
```docker
    docker run -p 3000:3000 my-docker-app
```


This command tells Docker to run the container and map port 3000 on your machine to port 3000 inside the container.

You can now visit http://localhost:3000 in your browser, and you should see the message "Hello, Docker!".

### Pushing to Docker Hub (Optional)
First, tag the image:
```docker
    docker tag my-docker-app your-docker-username/my-docker-app
```

Then, push it to Docker Hub:
```docker
    docker push your-docker-username/my-docker-app
```
