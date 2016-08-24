# system-admin-server

## Install

To enable design mode on your node application, install the packages:

```sh
// install system runtime module
$ npm install system-runtime --save

// install admin runtime module
$ npm install system-admin-server --save
```

Then:

```js
// require system runtime
var runtime = require('system-runtime');

// install admin system
var id = runtime.install('system-admin-server');

// start admin system
runtime.start(id);
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
