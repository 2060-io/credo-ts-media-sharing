# Aries JavaScript Media Sharing extension module

> **Deprecation notice:** Development has been moved to https://github.com/2060-io/credo-ts-didcomm-ext. New NPM package name is @2060.io/credo-ts-didcomm-media-sharing

This module is used to provide an Aries Agent built with Aries Framework JavaScript means to manage [Media Sharing protocol](https://github.com/genaris/didcomm.org/tree/feat/media-sharing/site/content/protocols/media-sharing/1.0).

It's conceived as an extension module for Aries Framework JavaScript which can be injected to an existing agent instance:

```ts
import { MediaSharingModule } from 'credo-ts-media-sharing'

const agent = new Agent({
  config: {
    /* agent config */
  },
  dependencies,
  modules: { media: new MediaSharingModule() },
})
```

Once instantiated, media module API can be accessed under `agent.modules.media` namespace

## Usage

### Sending a media file

![](./doc/diagrams/sender.png)

### Receiving a media file

![](./doc/diagrams/recipient.png)

> **TODO**
