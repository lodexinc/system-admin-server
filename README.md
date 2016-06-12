# system-admin-server

## Install

To enable design mode on your application, just require *system-admin-server* module in your application, and run it:

```js
// to use 'require' in system-admin-server module
global.require = require;

var admin = require('system-admin-server');

// run admin system
var systemId = runtime.require('db').system(admin);
runtime.require(systemId).main();
```

## Design

* Launch [System Designer](https://system-designer.github.io),
* open the *Configuration* panel,
* select *Server-side* as value for *Type of debugging*,
* set `http://localhost` as value for *Url of the server to debug*,
* click on the design button (the target icon),
* a panel *A system has been found* is shown
* click on *OK*.

The system running in node will be then imported in [System Designer](https://system-designer.github.io).

All your modifications to the current system in [System Designer](https://system-designer.github.io) will be injected into the server. 
