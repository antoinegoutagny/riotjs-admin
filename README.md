
![](https://moot.it/riotjs/demo/img/riotjslogo@2x.png)

## Riot.js demo application

This is a demo single-page demo application made with Riot.js. It's a generic skeleton for an administration panel that shows the core concepts of modular client side development.

### Features
- actually something useful, just fork it and extend it to your needs
- plain and minimal UI
- authentication and session management
- small: ~10kb minified, including Riot (4kb gzipped)
- optional caching of server side requests


### Modular architecture
- one global variable `admin` to build modules
- modules can be included in no specific order (*.js)
- modules can be renamed/removed/modified on without breaking the app
- backend agnostic
- easy to maintain and extend, good for multiple developers


### Extendable
- Real API: try for example `admin().load("customers")` on console
- Promise based server calls for more fluent error handling
- Use app name to extend instead of a framework name: `admin(callback)`


### Planned
- real backend (firebase, hosted server, to be decided...)
- realtime channel
- tests for both UI and API layer
- documented API, including events


## Installation

Hit following commands to run the administration panel on the console

``` sh
bower install
npm install
./make.js gen
open index.html
./make.js watch
```

You should be able to modify JS and Stylus files and the concatenation and pre-compilation is automatically taken care of. Check make.js for more other targets than `watch`.


[Live version](https://moot.it/riotjs/demo/) &bull;
[Riot website](https://moot.it/riotjs/) &bull;
[Building modular applications with Riot.js](https://moot.it/riotjs/docs/) &bull;
[Original Riot blog post](https://moot.it/blog/technology/riotjs-the-1kb-mvp-framework.html)

