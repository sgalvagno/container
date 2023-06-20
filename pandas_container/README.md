

# Build the docker
```
docker build -t pandas-dev .
```

# Run the container
go in your folder project

```
docker run -it --name myapp --rm \
    --volume /$(pwd):/usr/src/app \
    --net=host pandas-dev \
    -e LOCAL_USER_ID=`id -u $USER`
    bash
```

replace or not _myapp_ by your custom choice


# Jump in your container

```docker exec -it myapp bash```


# Comment

If you don't need pandas use python_container
