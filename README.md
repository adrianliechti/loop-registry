# Simple Docker Registry

## Usage

```bash
docker build . --tag loop-registry
docker run -it --rm -p 8080:5000 loop-registry
```

```bash
# pull sample image
docker pull nginx:latest

# tag image for registry
docker tag nginx:latest localhost:8080/nginx:latest

# push image to registry
docker push localhost:8080/nginx:latest
```