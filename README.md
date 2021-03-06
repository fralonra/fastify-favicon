# fastify-favicon
Fastify Plugin to serve default favicon.

With this plugin, Fastify will have a route configured for `/favicon.ico` requests.


## Usage

```js
const fastify = require('fastify')()

// example without specifying options, searching favicon.ico from project root, otherwise returning a default favicon
fastify.register(require('fastify-favicon'))
// or
// example with custom URL
fastify.register(require('fastify-favicon') {path: '/path/where/favicon/served'})

fastify.listen(3000)
// curl 127.0.0.1:3000/favicon.ico => returning the image, and no thrown error
```

## Requirements

Fastify 0.43.0 or later.


## License

Licensed under [Apache-2.0](./LICENSE).

----
