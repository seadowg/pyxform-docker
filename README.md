# pyxform-docker

Docker image for pyxform development.

## Using

From your local pyxform repo you can boot the environment with the codebase as a shared volume using:

```bash
docker run -it \
  --entrypoint /bin/bash \
  -v "$(pwd)":/pyxform \
  --workdir /pyxform \
  seadowg/pyxform
```
