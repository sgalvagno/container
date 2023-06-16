# Choose your lib
Put into requirement.txt the list of libraries you need for your project


# Build the docker
```
docker build -t python-dev .
```

# Run the container
go in your folder project

```
docker run -it --name myapp --rm \
    --volume $(pwd):/usr/src/app \
    --net=host myapp-dev:latest \
    sh
```

replace or not _myapp_ by your custom choice


# Jump in you container

```docker exec -it myapp bash```

