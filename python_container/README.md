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
    --volume /$(pwd):/usr/src/app \
    --net=host python-dev \
    bash
```

replace or not _myapp_ by your custom choice


# Jump in your container

```docker exec -it myapp bash```


# Issue
At this time I cannot install Pandas
then use Dockerfile in pandas_container folder.


