# bsp-env

This repo allows to create a docker container for BSP development based on Ubuntu with Yocto or Buildroot.


### Build image
```
docker build --build-arg "host_uid=$(id -u)" --build-arg "host_gid=$(id -g)" -t bsp-env -f <filename> .
```

### Run container

```
docker run -it -v $(pwd):/home bsp-env
```
