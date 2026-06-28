#### How to Build

```bash
docker buildx use multiarch-builder

docker buildx build \
  --platform linux/amd64,linux/arm64 \
  -t {YOUR_USERNAME}/config-store:1.0.0 \
  --push \
  .
```

#### How to Test on Local

```bash
$ docker compose up --build --watch
```
