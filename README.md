# system-admin-server

To enable design mode on your application, just require *system-admin-server* module in your application, and run it:

```js
var admin = require('system-admin-server');

// run admin system
var systemId = runtime.require('db').system(admin);
runtime.require(systemId).main();
```