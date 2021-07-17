# url-redirect-proxy

## `envoy` proxy

```
docker run --name=envoyproxy -it \
  -p 8080:10000 \
  -v $(pwd)/envoy/envoy.yaml:/etc/envoy/envoy.yaml \
  envoyproxy/envoy-distroless:v1.19.0
```

## `nginx` proxy

FIXME