<sup>If you're looking for the officially supported bindings for JavaScript see the [pymavlink](https://github.com/ArduPilot/pymavlink/tree/master/generator/javascript) project.</sup>

# MavLink Parser for the browser

Mavlink-parser-browserify is a copy of [node-mavlink](https://github.com/ArduPilot/node-mavlink). Unfortunately, the original node-mavlink library has a dependency on the [node UDP/datagram sockets module (dgram)](https://nodejs.org/api/dgram.html). This is an issue when trying to run node-mavlink in a browser-only environment from Webpack 5 lost polyfill.

This work is simply the [node-mavlink](https://github.com/ArduPilot/node-mavlink) striped of its dependency on dgram (and the functionalities linked to it).