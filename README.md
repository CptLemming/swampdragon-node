# [SwampDragon](http://swampdragon.net) node client

A modified version of the SwampDragon javascript client to play nicer with node.

Changes:
- Include SockJS client (removes need for browserify-shim)
- Does *not* connect automatically
- DataMapper modified to support CommonJS

```
var SwampDragon = require('swampdragon-node');

SwampDragon.connect({
    host: 'http://localhost:9999',
    endpoint: '/data'
});
```
