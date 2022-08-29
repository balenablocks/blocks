![banner](https://raw.githubusercontent.com/balenablocks/blocks/master/docs/images/banner.png)

Reducing the friction for IOT application developers by providing drop-in chunks of functionality.

## Highlights
* **Pre-built containers**: Just drop them into your IOT projects
* **Provide functionality**: Need a containerised browser? Just drop in the [browser block](https://github.com/balenablocks/browser)!
* **Intelligent and opinionated**: Blocks discover each other and work together automatically.

## Motivation
Blocks are a concept that came out of the [labs](https://github.com/balenalabs) at balena.

![blocks factory](https://raw.githubusercontent.com/balenablocks/blocks/master/docs/images/factory.png)

Balena's mission is to reduce friction for fleet owners and unlock the power of physical computing. Blocks contribute to this by removing friction for developers of IOT applications by providing pre-built chunks of functionality. They enable application developers to focus only on the code they need to write, and rely on the blocks to provide everything else.

## Usage
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

For more details and advanced scenarios head over to the [usage](/docs/01-usage.md) section of the docs.