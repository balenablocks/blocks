# How to use blocks

You can find the blocks that are available to use on [balenaHub](https://hub.balena.io/blocks). Each one will have an `image reference` like this:

![browser reference](https://raw.githubusercontent.com/balenablocks/blocks/master/docs/images/browser-block-image-reference.png)

You can use this `image reference` in two ways; in your `docker-compose.yml` file, or in a `dockerfile`:

### Docker-Compose
The `image reference` is added under services:

```yaml
version: '2.1'

services:
  browser:
    image: bhcr.io/balenablocks/browser-aarch64
```

### Dockerfile
The `image reference` is used in the `FROM` directive:

```
FROM bhcr.io/balenablocks/browser-aarch64 as base
```

