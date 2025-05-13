# Dockerfile_Collections
This repository contains several Dockerfiles for different environments which will be often used.

## torch-cpu
- Build Image
```
docker build -f Dockerfile.torch-cpu -t torch_cpu_env .
```
- Run Container
```
docker run -it -p 8888:8888 \
> --name torch-cpu \
> -v ~/study_ws:/workspace \
> torch_cpu_env
```

> Don't forget mkdir study_ws folder before run container