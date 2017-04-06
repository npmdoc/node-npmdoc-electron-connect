# api documentation for  [electron-connect (v0.6.1)](https://github.com/Quramy/electron-connect)  [![npm package](https://img.shields.io/npm/v/npmdoc-electron-connect.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-electron-connect) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-electron-connect.svg)](https://travis-ci.org/npmdoc/node-npmdoc-electron-connect)
#### Livereload tools for Electron development

[![NPM](https://nodei.co/npm/electron-connect.png?downloads=true)](https://www.npmjs.com/package/electron-connect)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-connect/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-electron-connect_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-connect/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-electron-connect/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-electron-connect/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Quramy",
        "email": "yosuke.kurami@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/Quramy/electron-connect/issues"
    },
    "contributors": [
        {
            "name": "Quramy",
            "email": "yosuke.kurami@gmail.com"
        },
        {
            "name": "Sreekanth",
            "email": "s.sreekanth@outlook.com"
        }
    ],
    "dependencies": {
        "cross-spawn": "^5.0.1",
        "lodash": "^4.17.2",
        "tree-kill": "^1.1.0",
        "ws": "^1.1.1"
    },
    "description": "Livereload tools for Electron development",
    "devDependencies": {
        "electron": "^1.4.7",
        "gulp": "^3.9.1",
        "gulp-mocha": "^3.0.1",
        "spectron": "^3.4.0"
    },
    "directories": {},
    "dist": {
        "shasum": "6dce9093cdfe7b06941dfcc487efa4a1b6df0b4e",
        "tarball": "https://registry.npmjs.org/electron-connect/-/electron-connect-0.6.1.tgz"
    },
    "gitHead": "2dbef3cd01f261662e6642705c32b71f8f2baf55",
    "homepage": "https://github.com/Quramy/electron-connect",
    "keywords": [
        "electron",
        "livereload",
        "gulp"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "quramy",
            "email": "yosuke.kurami@gmail.com"
        }
    ],
    "name": "electron-connect",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Quramy/electron-connect.git"
    },
    "scripts": {
        "test": "gulp test"
    },
    "version": "0.6.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module electron-connect](#apidoc.module.electron-connect)
1.  [function <span class="apidocSignatureSpan">electron-connect.</span>socketWrapper (ws)](#apidoc.element.electron-connect.socketWrapper)
1.  object <span class="apidocSignatureSpan">electron-connect.</span>client
1.  object <span class="apidocSignatureSpan">electron-connect.</span>server
1.  object <span class="apidocSignatureSpan">electron-connect.</span>socketWrapper.prototype
1.  object <span class="apidocSignatureSpan">electron-connect.</span>util

#### [module electron-connect.client](#apidoc.module.electron-connect.client)
1.  [function <span class="apidocSignatureSpan">electron-connect.client.</span>create (browserWindow, options, cb)](#apidoc.element.electron-connect.client.create)

#### [module electron-connect.server](#apidoc.module.electron-connect.server)
1.  [function <span class="apidocSignatureSpan">electron-connect.server.</span>create (options)](#apidoc.element.electron-connect.server.create)

#### [module electron-connect.socketWrapper](#apidoc.module.electron-connect.socketWrapper)
1.  [function <span class="apidocSignatureSpan">electron-connect.</span>socketWrapper (ws)](#apidoc.element.electron-connect.socketWrapper.socketWrapper)
1.  [function <span class="apidocSignatureSpan">electron-connect.socketWrapper.</span>add (wrapper)](#apidoc.element.electron-connect.socketWrapper.add)
1.  [function <span class="apidocSignatureSpan">electron-connect.socketWrapper.</span>broadcast (type, data)](#apidoc.element.electron-connect.socketWrapper.broadcast)
1.  [function <span class="apidocSignatureSpan">electron-connect.socketWrapper.</span>delete (id)](#apidoc.element.electron-connect.socketWrapper.delete)
1.  [function <span class="apidocSignatureSpan">electron-connect.socketWrapper.</span>get (id)](#apidoc.element.electron-connect.socketWrapper.get)

#### [module electron-connect.socketWrapper.prototype](#apidoc.module.electron-connect.socketWrapper.prototype)
1.  [function <span class="apidocSignatureSpan">electron-connect.socketWrapper.prototype.</span>clearAll ()](#apidoc.element.electron-connect.socketWrapper.prototype.clearAll)
1.  [function <span class="apidocSignatureSpan">electron-connect.socketWrapper.prototype.</span>get (key)](#apidoc.element.electron-connect.socketWrapper.prototype.get)
1.  [function <span class="apidocSignatureSpan">electron-connect.socketWrapper.prototype.</span>on ()](#apidoc.element.electron-connect.socketWrapper.prototype.on)
1.  [function <span class="apidocSignatureSpan">electron-connect.socketWrapper.prototype.</span>set (key, value)](#apidoc.element.electron-connect.socketWrapper.prototype.set)

#### [module electron-connect.util](#apidoc.module.electron-connect.util)
1.  [function <span class="apidocSignatureSpan">electron-connect.util.</span>getIdFromUrl (url)](#apidoc.element.electron-connect.util.getIdFromUrl)
1.  [function <span class="apidocSignatureSpan">electron-connect.util.</span>sendMessage (socket, type, data)](#apidoc.element.electron-connect.util.sendMessage)
1.  number <span class="apidocSignatureSpan">electron-connect.util.</span>LOG_LEVEL_INFO
1.  number <span class="apidocSignatureSpan">electron-connect.util.</span>LOG_LEVEL_VERBOSE
1.  number <span class="apidocSignatureSpan">electron-connect.util.</span>LOG_LEVEL_WARNING



# <a name="apidoc.module.electron-connect"></a>[module electron-connect](#apidoc.module.electron-connect)

#### <a name="apidoc.element.electron-connect.socketWrapper"></a>[function <span class="apidocSignatureSpan">electron-connect.</span>socketWrapper (ws)](#apidoc.element.electron-connect.socketWrapper)
- description and source-code
```javascript
socketWrapper = function (ws) {
  this._socket = ws;
  if(ws && ws.upgradeReq) {
    this.id = util.getIdFromUrl(ws.upgradeReq.url);
  }
  this.sendMessage = createReply(ws);
  if(!registry[this.id]) {
    registry[this.id] = {};
  }
  SocketWrapper.add(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-connect.client"></a>[module electron-connect.client](#apidoc.module.electron-connect.client)

#### <a name="apidoc.element.electron-connect.client.create"></a>[function <span class="apidocSignatureSpan">electron-connect.client.</span>create (browserWindow, options, cb)](#apidoc.element.electron-connect.client.create)
- description and source-code
```javascript
create = function (browserWindow, options, cb) {
  return new Client().join(browserWindow, options, cb);
}
```
- example usage
```shell
...
### Server
Here is an example creating a server in [gulpfile](http://gulpjs.com/).

'''js
'use strict';

var gulp = require('gulp');
var electron = require('electron-connect').server.create();

gulp.task('serve', function () {

// Start browser process
electron.start();

// Restart browser process
...
```



# <a name="apidoc.module.electron-connect.server"></a>[module electron-connect.server](#apidoc.module.electron-connect.server)

#### <a name="apidoc.element.electron-connect.server.create"></a>[function <span class="apidocSignatureSpan">electron-connect.server.</span>create (options)](#apidoc.element.electron-connect.server.create)
- description and source-code
```javascript
create = function (options) {
  var electron;
  if(options && options.useGlobalElectron) {
    electron = 'electron';
  } else {
    try {
      electron = require('electron');
    } catch (e) {
      if(e.code === 'MODULE_NOT_FOUND') {
        electron = 'electron';
      }
    }
  }
  var opt = _.merge({
    stopOnClose: false,
    electron: electron,
    path: process.cwd(),
    port: 30080,
    logLevel: util.LOG_LEVEL_INFO,
    spawnOpt: {stdio: 'inherit'}
  }, options || {});
  return new ProcessManager().init(opt);
}
```
- example usage
```shell
...
### Server
Here is an example creating a server in [gulpfile](http://gulpjs.com/).

'''js
'use strict';

var gulp = require('gulp');
var electron = require('electron-connect').server.create();

gulp.task('serve', function () {

// Start browser process
electron.start();

// Restart browser process
...
```



# <a name="apidoc.module.electron-connect.socketWrapper"></a>[module electron-connect.socketWrapper](#apidoc.module.electron-connect.socketWrapper)

#### <a name="apidoc.element.electron-connect.socketWrapper.socketWrapper"></a>[function <span class="apidocSignatureSpan">electron-connect.</span>socketWrapper (ws)](#apidoc.element.electron-connect.socketWrapper.socketWrapper)
- description and source-code
```javascript
socketWrapper = function (ws) {
  this._socket = ws;
  if(ws && ws.upgradeReq) {
    this.id = util.getIdFromUrl(ws.upgradeReq.url);
  }
  this.sendMessage = createReply(ws);
  if(!registry[this.id]) {
    registry[this.id] = {};
  }
  SocketWrapper.add(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-connect.socketWrapper.add"></a>[function <span class="apidocSignatureSpan">electron-connect.socketWrapper.</span>add (wrapper)](#apidoc.element.electron-connect.socketWrapper.add)
- description and source-code
```javascript
add = function (wrapper) {
  repo[wrapper.id] = wrapper;
}
```
- example usage
```shell
...
  if(ws && ws.upgradeReq) {
    this.id = util.getIdFromUrl(ws.upgradeReq.url);
  }
  this.sendMessage = createReply(ws);
  if(!registry[this.id]) {
    registry[this.id] = {};
  }
  SocketWrapper.add(this);
};

SocketWrapper.get = function (id) {
  return repo[id];
};

SocketWrapper.add = function (wrapper) {
...
```

#### <a name="apidoc.element.electron-connect.socketWrapper.broadcast"></a>[function <span class="apidocSignatureSpan">electron-connect.socketWrapper.</span>broadcast (type, data)](#apidoc.element.electron-connect.socketWrapper.broadcast)
- description and source-code
```javascript
broadcast = function (type, data) {
  for(var id in repo) {
    repo[id].sendMessage(type, data);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-connect.socketWrapper.delete"></a>[function <span class="apidocSignatureSpan">electron-connect.socketWrapper.</span>delete (id)](#apidoc.element.electron-connect.socketWrapper.delete)
- description and source-code
```javascript
delete = function (id) {
  delete repo[id];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-connect.socketWrapper.get"></a>[function <span class="apidocSignatureSpan">electron-connect.socketWrapper.</span>get (id)](#apidoc.element.electron-connect.socketWrapper.get)
- description and source-code
```javascript
get = function (id) {
  return repo[id];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-connect.socketWrapper.prototype"></a>[module electron-connect.socketWrapper.prototype](#apidoc.module.electron-connect.socketWrapper.prototype)

#### <a name="apidoc.element.electron-connect.socketWrapper.prototype.clearAll"></a>[function <span class="apidocSignatureSpan">electron-connect.socketWrapper.prototype.</span>clearAll ()](#apidoc.element.electron-connect.socketWrapper.prototype.clearAll)
- description and source-code
```javascript
clearAll = function () {
  registry[this.id] = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-connect.socketWrapper.prototype.get"></a>[function <span class="apidocSignatureSpan">electron-connect.socketWrapper.prototype.</span>get (key)](#apidoc.element.electron-connect.socketWrapper.prototype.get)
- description and source-code
```javascript
get = function (key) {
  if(registry[this.id]){
    return registry[this.id][key];
  }
  return;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-connect.socketWrapper.prototype.on"></a>[function <span class="apidocSignatureSpan">electron-connect.socketWrapper.prototype.</span>on ()](#apidoc.element.electron-connect.socketWrapper.prototype.on)
- description and source-code
```javascript
on = function () {
  this._socket.on.apply(this._socket, arguments);
  return this;
}
```
- example usage
```shell
...
'''js
'use strict';

var app = require('app');
var BrowserWindow = require('browser-window');
var client = require('electron-connect').client;

app.on('ready', function () {
var mainWindow = new BrowserWindow({
  width: 400,
  height: 300
});
mainWindow.loadUrl('file://' + __dirname + '/index.html');

// Connect to server process
...
```

#### <a name="apidoc.element.electron-connect.socketWrapper.prototype.set"></a>[function <span class="apidocSignatureSpan">electron-connect.socketWrapper.prototype.</span>set (key, value)](#apidoc.element.electron-connect.socketWrapper.prototype.set)
- description and source-code
```javascript
set = function (key, value) {
  if(registry[this.id]){
    registry[this.id][key] = value;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-connect.util"></a>[module electron-connect.util](#apidoc.module.electron-connect.util)

#### <a name="apidoc.element.electron-connect.util.getIdFromUrl"></a>[function <span class="apidocSignatureSpan">electron-connect.util.</span>getIdFromUrl (url)](#apidoc.element.electron-connect.util.getIdFromUrl)
- description and source-code
```javascript
getIdFromUrl = function (url) {
  var matched = url.match(/\?window_id=([^&])/);
  return matched && matched[1];
}
```
- example usage
```shell
...
};

var repo = {};
var registry = {};
var SocketWrapper = function (ws) {
  this._socket = ws;
  if(ws && ws.upgradeReq) {
    this.id = util.getIdFromUrl(ws.upgradeReq.url);
  }
  this.sendMessage = createReply(ws);
  if(!registry[this.id]) {
    registry[this.id] = {};
  }
  SocketWrapper.add(this);
};
...
```

#### <a name="apidoc.element.electron-connect.util.sendMessage"></a>[function <span class="apidocSignatureSpan">electron-connect.util.</span>sendMessage (socket, type, data)](#apidoc.element.electron-connect.util.sendMessage)
- description and source-code
```javascript
sendMessage = function (socket, type, data) {
  if(!type || !socket || socket.readyState !== webSocket.OPEN) return;
  var obj = {type: type};
  if(data) obj.data = data;
  socket.send(JSON.stringify(obj));
}
```
- example usage
```shell
...

'use strict';

var util = require('./util');

var createReply = function (ws) {
return function (type, data) {
  return util.sendMessage(ws, type, data);
};
};

var repo = {};
var registry = {};
var SocketWrapper = function (ws) {
this._socket = ws;
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
