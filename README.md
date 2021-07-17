# url-redirect-proxy

## `envoy` proxy

Without `Dockerfile`:
```
docker run --name=envoyproxy -it \
  -p 8080:10000 \
  -v $(pwd)/envoy/envoy.yaml:/etc/envoy/envoy.yaml \
  envoyproxy/envoy-distroless:v1.19.0
```

With `Dockerfile`:
```
docker build -t envoyproxy .
docker run --name=envoyproxy -it \
  -p 8080:10000 \
  envoyproxy
```

## `nginx` proxy

FIXME