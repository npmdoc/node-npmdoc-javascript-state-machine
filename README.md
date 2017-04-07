# api documentation for  [javascript-state-machine (v2.4.0)](https://github.com/jakesgordon/javascript-state-machine)  [![npm package](https://img.shields.io/npm/v/npmdoc-javascript-state-machine.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-javascript-state-machine) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-javascript-state-machine.svg)](https://travis-ci.org/npmdoc/node-npmdoc-javascript-state-machine)
#### A simple finite state machine library

[![NPM](https://nodei.co/npm/javascript-state-machine.png?downloads=true)](https://www.npmjs.com/package/javascript-state-machine)

[![apidoc](https://npmdoc.github.io/node-npmdoc-javascript-state-machine/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-javascript-state-machine_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-javascript-state-machine/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-javascript-state-machine/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-javascript-state-machine/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jake Gordon",
        "email": "jake@codeincomplete.com"
    },
    "bugs": {
        "url": "https://github.com/jakesgordon/javascript-state-machine/issues"
    },
    "dependencies": {},
    "description": "A simple finite state machine library",
    "devDependencies": {
        "local-web-server": "~1.2.6",
        "qunit": "~0.9.1",
        "uglify-js": "^2.7.4"
    },
    "directories": {},
    "dist": {
        "shasum": "d8be31ec38f24ac1a1832f0b672fc3cd5f79c96e",
        "tarball": "https://registry.npmjs.org/javascript-state-machine/-/javascript-state-machine-2.4.0.tgz"
    },
    "gitHead": "c7538b4fce486a84de7a456b72ce7dc15201c818",
    "homepage": "https://github.com/jakesgordon/javascript-state-machine",
    "keywords": [
        "state machine",
        "server",
        "client"
    ],
    "main": "state-machine.js",
    "maintainers": [
        {
            "name": "jakesgordon",
            "email": "jakesgordon@gmail.com"
        }
    ],
    "name": "javascript-state-machine",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/jakesgordon/javascript-state-machine.git"
    },
    "scripts": {
        "minify": "uglifyjs state-machine.js --output state-machine.min.js --compress --mangle --stats",
        "start": "ws --rewrite '/test -> /test/'",
        "test": "node test/runner"
    },
    "version": "2.4.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module javascript-state-machine](#apidoc.module.javascript-state-machine)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>afterAnyEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.afterAnyEvent)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>afterEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.afterEvent)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>afterThisEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.afterThisEvent)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>beforeAnyEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.beforeAnyEvent)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>beforeEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.beforeEvent)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>beforeThisEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.beforeThisEvent)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>buildEvent (name, map)](#apidoc.element.javascript-state-machine.buildEvent)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>changeState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.changeState)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>create (cfg, target)](#apidoc.element.javascript-state-machine.create)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>doCallback (fsm, func, name, from, to, args)](#apidoc.element.javascript-state-machine.doCallback)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>enterAnyState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.enterAnyState)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>enterState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.enterState)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>enterThisState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.enterThisState)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>leaveAnyState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.leaveAnyState)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>leaveState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.leaveState)
1.  [function <span class="apidocSignatureSpan">javascript-state-machine.</span>leaveThisState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.leaveThisState)
1.  object <span class="apidocSignatureSpan">javascript-state-machine.</span>Error
1.  object <span class="apidocSignatureSpan">javascript-state-machine.</span>Result
1.  object <span class="apidocSignatureSpan">javascript-state-machine.</span>StateMachine
1.  string <span class="apidocSignatureSpan">javascript-state-machine.</span>ASYNC
1.  string <span class="apidocSignatureSpan">javascript-state-machine.</span>VERSION
1.  string <span class="apidocSignatureSpan">javascript-state-machine.</span>WILDCARD



# <a name="apidoc.module.javascript-state-machine"></a>[module javascript-state-machine](#apidoc.module.javascript-state-machine)

#### <a name="apidoc.element.javascript-state-machine.afterAnyEvent"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>afterAnyEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.afterAnyEvent)
- description and source-code
```javascript
afterAnyEvent = function (fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onafterevent'] || fsm['onevent'],      name, from
, to, args); }
```
- example usage
```shell
...
  if ((false === StateMachine.beforeThisEvent(fsm, name, from, to, args)) ||
      (false === StateMachine.beforeAnyEvent( fsm, name, from, to, args)))
    return false;
},

afterEvent: function(fsm, name, from, to, args) {
  StateMachine.afterThisEvent(fsm, name, from, to, args);
  StateMachine.afterAnyEvent( fsm, name, from, to, args);
},

leaveState: function(fsm, name, from, to, args) {
  var specific = StateMachine.leaveThisState(fsm, name, from, to, args),
      general  = StateMachine.leaveAnyState( fsm, name, from, to, args);
  if ((false === specific) || (false === general))
    return false;
...
```

#### <a name="apidoc.element.javascript-state-machine.afterEvent"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>afterEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.afterEvent)
- description and source-code
```javascript
afterEvent = function (fsm, name, from, to, args) {
  StateMachine.afterThisEvent(fsm, name, from, to, args);
  StateMachine.afterAnyEvent( fsm, name, from, to, args);
}
```
- example usage
```shell
...
if (this.cannot(name))
  return this.error(name, from, to, args, StateMachine.Error.INVALID_TRANSITION, "event " + name + " inappropriate in current state
 " + this.current);

if (false === StateMachine.beforeEvent(this, name, from, to, args))
  return StateMachine.Result.CANCELLED;

if (from === to) {
  StateMachine.afterEvent(this, name, from, to, args);
  return StateMachine.Result.NOTRANSITION;
}

// prepare a transition method for use EITHER lower down, or by caller if they want an async transition (indicated by an ASYNC return
 value from leaveState)
var fsm = this;
this.transition = function() {
  fsm.transition = null; // this method should only ever be called once
...
```

#### <a name="apidoc.element.javascript-state-machine.afterThisEvent"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>afterThisEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.afterThisEvent)
- description and source-code
```javascript
afterThisEvent = function (fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onafter'  + name] || fsm['on' + name], name, from
, to, args); }
```
- example usage
```shell
...
beforeEvent: function(fsm, name, from, to, args) {
  if ((false === StateMachine.beforeThisEvent(fsm, name, from, to, args)) ||
      (false === StateMachine.beforeAnyEvent( fsm, name, from, to, args)))
    return false;
},

afterEvent: function(fsm, name, from, to, args) {
  StateMachine.afterThisEvent(fsm, name, from, to, args);
  StateMachine.afterAnyEvent( fsm, name, from, to, args);
},

leaveState: function(fsm, name, from, to, args) {
  var specific = StateMachine.leaveThisState(fsm, name, from, to, args),
      general  = StateMachine.leaveAnyState( fsm, name, from, to, args);
  if ((false === specific) || (false === general))
...
```

#### <a name="apidoc.element.javascript-state-machine.beforeAnyEvent"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>beforeAnyEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.beforeAnyEvent)
- description and source-code
```javascript
beforeAnyEvent = function (fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onbeforeevent'],                       name, from
, to, args); }
```
- example usage
```shell
...
beforeThisEvent: function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onbefore' + name],
name, from, to, args); },
afterThisEvent:  function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onafter'  + name] || fsm['on' +
name], name, from, to, args); },
leaveThisState:  function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onleave'  + from],
name, from, to, args); },
enterThisState:  function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onenter'  + to]   || fsm['on' +
to],   name, from, to, args); },

beforeEvent: function(fsm, name, from, to, args) {
  if ((false === StateMachine.beforeThisEvent(fsm, name, from, to, args)) ||
      (false === StateMachine.beforeAnyEvent( fsm, name, from, to, args)))
    return false;
},

afterEvent: function(fsm, name, from, to, args) {
  StateMachine.afterThisEvent(fsm, name, from, to, args);
  StateMachine.afterAnyEvent( fsm, name, from, to, args);
},
...
```

#### <a name="apidoc.element.javascript-state-machine.beforeEvent"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>beforeEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.beforeEvent)
- description and source-code
```javascript
beforeEvent = function (fsm, name, from, to, args) {
  if ((false === StateMachine.beforeThisEvent(fsm, name, from, to, args)) ||
      (false === StateMachine.beforeAnyEvent( fsm, name, from, to, args)))
    return false;
}
```
- example usage
```shell
...

if (this.transition)
  return this.error(name, from, to, args, StateMachine.Error.PENDING_TRANSITION, "event " + name + " inappropriate because previous
 transition did not complete");

if (this.cannot(name))
  return this.error(name, from, to, args, StateMachine.Error.INVALID_TRANSITION, "event " + name + " inappropriate in current state
 " + this.current);

if (false === StateMachine.beforeEvent(this, name, from, to, args))
  return StateMachine.Result.CANCELLED;

if (from === to) {
  StateMachine.afterEvent(this, name, from, to, args);
  return StateMachine.Result.NOTRANSITION;
}
...
```

#### <a name="apidoc.element.javascript-state-machine.beforeThisEvent"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>beforeThisEvent (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.beforeThisEvent)
- description and source-code
```javascript
beforeThisEvent = function (fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onbefore' + name],                     name, from
, to, args); }
```
- example usage
```shell
...

beforeThisEvent: function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onbefore' + name],
name, from, to, args); },
afterThisEvent:  function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onafter'  + name] || fsm['on' +
name], name, from, to, args); },
leaveThisState:  function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onleave'  + from],
name, from, to, args); },
enterThisState:  function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onenter'  + to]   || fsm['on' +
to],   name, from, to, args); },

beforeEvent: function(fsm, name, from, to, args) {
  if ((false === StateMachine.beforeThisEvent(fsm, name, from, to, args)) ||
      (false === StateMachine.beforeAnyEvent( fsm, name, from, to, args)))
    return false;
},

afterEvent: function(fsm, name, from, to, args) {
  StateMachine.afterThisEvent(fsm, name, from, to, args);
  StateMachine.afterAnyEvent( fsm, name, from, to, args);
...
```

#### <a name="apidoc.element.javascript-state-machine.buildEvent"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>buildEvent (name, map)](#apidoc.element.javascript-state-machine.buildEvent)
- description and source-code
```javascript
buildEvent = function (name, map) {
  return function() {

    var from  = this.current;
    var to    = map[from] || (map[StateMachine.WILDCARD] != StateMachine.WILDCARD ? map[StateMachine.WILDCARD] : from) || from;
    var args  = Array.prototype.slice.call(arguments); // turn arguments into pure array

    if (this.transition)
      return this.error(name, from, to, args, StateMachine.Error.PENDING_TRANSITION, "event " + name + " inappropriate because previous
 transition did not complete");

    if (this.cannot(name))
      return this.error(name, from, to, args, StateMachine.Error.INVALID_TRANSITION, "event " + name + " inappropriate in current
 state " + this.current);

    if (false === StateMachine.beforeEvent(this, name, from, to, args))
      return StateMachine.Result.CANCELLED;

    if (from === to) {
      StateMachine.afterEvent(this, name, from, to, args);
      return StateMachine.Result.NOTRANSITION;
    }

    // prepare a transition method for use EITHER lower down, or by caller if they want an async transition (indicated by an ASYNC
 return value from leaveState)
    var fsm = this;
    this.transition = function() {
      fsm.transition = null; // this method should only ever be called once
      fsm.current = to;
      StateMachine.enterState( fsm, name, from, to, args);
      StateMachine.changeState(fsm, name, from, to, args);
      StateMachine.afterEvent( fsm, name, from, to, args);
      return StateMachine.Result.SUCCEEDED;
    };
    this.transition.cancel = function() { // provide a way for caller to cancel async transition if desired (issue #22)
      fsm.transition = null;
      StateMachine.afterEvent(fsm, name, from, to, args);
    }

    var leave = StateMachine.leaveState(this, name, from, to, args);
    if (false === leave) {
      this.transition = null;
      return StateMachine.Result.CANCELLED;
    }
    else if (StateMachine.ASYNC === leave) {
      return StateMachine.Result.PENDING;
    }
    else {
      if (this.transition) // need to check in case user manually called transition() but forgot to return StateMachine.ASYNC
        return this.transition();
    }

  };
}
```
- example usage
```shell
...
}

for(var n = 0 ; n < events.length ; n++)
  add(events[n]);

for(var name in map) {
  if (map.hasOwnProperty(name))
    fsm[name] = StateMachine.buildEvent(name, map[name]);
}

for(var name in callbacks) {
  if (callbacks.hasOwnProperty(name))
    fsm[name] = callbacks[name]
}
...
```

#### <a name="apidoc.element.javascript-state-machine.changeState"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>changeState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.changeState)
- description and source-code
```javascript
changeState = function (fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onchangestate'],                       name, from
, to, args); }
```
- example usage
```shell
...

// prepare a transition method for use EITHER lower down, or by caller if they want an async transition (indicated by an ASYNC return
 value from leaveState)
var fsm = this;
this.transition = function() {
  fsm.transition = null; // this method should only ever be called once
  fsm.current = to;
  StateMachine.enterState( fsm, name, from, to, args);
  StateMachine.changeState(fsm, name, from, to, args);
  StateMachine.afterEvent( fsm, name, from, to, args);
  return StateMachine.Result.SUCCEEDED;
};
this.transition.cancel = function() { // provide a way for caller to cancel async transition if desired (issue #22)
  fsm.transition = null;
  StateMachine.afterEvent(fsm, name, from, to, args);
}
...
```

#### <a name="apidoc.element.javascript-state-machine.create"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>create (cfg, target)](#apidoc.element.javascript-state-machine.create)
- description and source-code
```javascript
create = function (cfg, target) {

  var initial      = (typeof cfg.initial == 'string') ? { state: cfg.initial } : cfg.initial; // allow for a simple string, or an
 object with { state: 'foo', event: 'setup', defer: true|false }
  var terminal     = cfg.terminal || cfg['final'];
  var fsm          = target || cfg.target  || {};
  var events       = cfg.events || [];
  var callbacks    = cfg.callbacks || {};
  var map          = {}; // track state transitions allowed for an event { event: { from: [ to ] } }
  var transitions  = {}; // track events allowed from a state            { state: [ event ] }

  var add = function(e) {
    var from = Array.isArray(e.from) ? e.from : (e.from ? [e.from] : [StateMachine.WILDCARD]); // allow 'wildcard' transition if
 'from' is not specified
    map[e.name] = map[e.name] || {};
    for (var n = 0 ; n < from.length ; n++) {
      transitions[from[n]] = transitions[from[n]] || [];
      transitions[from[n]].push(e.name);

      map[e.name][from[n]] = e.to || from[n]; // allow no-op transition if 'to' is not specified
    }
    if (e.to)
      transitions[e.to] = transitions[e.to] || [];
  };

  if (initial) {
    initial.event = initial.event || 'startup';
    add({ name: initial.event, from: 'none', to: initial.state });
  }

  for(var n = 0 ; n < events.length ; n++)
    add(events[n]);

  for(var name in map) {
    if (map.hasOwnProperty(name))
      fsm[name] = StateMachine.buildEvent(name, map[name]);
  }

  for(var name in callbacks) {
    if (callbacks.hasOwnProperty(name))
      fsm[name] = callbacks[name]
  }

  fsm.current     = 'none';
  fsm.is          = function(state) { return Array.isArray(state) ? (state.indexOf(this.current) >= 0) : (this.current === state
); };
  fsm.can         = function(event) { return !this.transition && (map[event] !== undefined) && (map[event].hasOwnProperty(this.current
) || map[event].hasOwnProperty(StateMachine.WILDCARD)); }
  fsm.cannot      = function(event) { return !this.can(event); };
  fsm.transitions = function()      { return (transitions[this.current] || []).concat(transitions[StateMachine.WILDCARD] || []); };
  fsm.isFinished  = function()      { return this.is(terminal); };
  fsm.error       = cfg.error || function(name, from, to, args, error, msg, e) { throw e || msg; }; // default behavior when something
 unexpected happens is to throw an exception, but caller can override this behavior if desired (see github issue #3 and #17)
  fsm.states      = function() { return Object.keys(transitions).sort() };

  if (initial && !initial.defer)
    fsm[initial.event]();

  return fsm;

}
```
- example usage
```shell
...

Or for npm:

var StateMachine = require('javascript-state-machine');

In its simplest form, create a standalone state machine using:

var fsm = StateMachine.create({
  initial: 'green',
  events: [
    { name: 'warn',  from: 'green',  to: 'yellow' },
    { name: 'panic', from: 'yellow', to: 'red'    },
    { name: 'calm',  from: 'red',    to: 'yellow' },
    { name: 'clear', from: 'yellow', to: 'green'  }
]});
...
```

#### <a name="apidoc.element.javascript-state-machine.doCallback"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>doCallback (fsm, func, name, from, to, args)](#apidoc.element.javascript-state-machine.doCallback)
- description and source-code
```javascript
doCallback = function (fsm, func, name, from, to, args) {
  if (func) {
    try {
      return func.apply(fsm, [name, from, to].concat(args));
    }
    catch(e) {
      return fsm.error(name, from, to, args, StateMachine.Error.INVALID_CALLBACK, "an exception occurred in a caller-provided callback
 function", e);
    }
  }
}
```
- example usage
```shell
...
    }
    catch(e) {
      return fsm.error(name, from, to, args, StateMachine.Error.INVALID_CALLBACK, "an exception occurred in a caller-provided callback
 function", e);
    }
  }
},

beforeAnyEvent:  function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onbeforeevent'],
name, from, to, args); },
afterAnyEvent:   function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onafterevent'] || fsm['onevent'],
name, from, to, args); },
leaveAnyState:   function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onleavestate'],
name, from, to, args); },
enterAnyState:   function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onenterstate'] || fsm['onstate'],
name, from, to, args); },
changeState:     function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onchangestate'],
name, from, to, args); },

beforeThisEvent: function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onbefore' + name],
name, from, to, args); },
afterThisEvent:  function(fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onafter'  + name] || fsm['on' +
name], name, from, to, args); },
...
```

#### <a name="apidoc.element.javascript-state-machine.enterAnyState"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>enterAnyState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.enterAnyState)
- description and source-code
```javascript
enterAnyState = function (fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onenterstate'] || fsm['onstate'],      name, from
, to, args); }
```
- example usage
```shell
...
    return false;
  else if ((StateMachine.ASYNC === specific) || (StateMachine.ASYNC === general))
    return StateMachine.ASYNC;
},

enterState: function(fsm, name, from, to, args) {
  StateMachine.enterThisState(fsm, name, from, to, args);
  StateMachine.enterAnyState( fsm, name, from, to, args);
},

//===========================================================================

buildEvent: function(name, map) {
  return function() {
...
```

#### <a name="apidoc.element.javascript-state-machine.enterState"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>enterState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.enterState)
- description and source-code
```javascript
enterState = function (fsm, name, from, to, args) {
  StateMachine.enterThisState(fsm, name, from, to, args);
  StateMachine.enterAnyState( fsm, name, from, to, args);
}
```
- example usage
```shell
...
}

// prepare a transition method for use EITHER lower down, or by caller if they want an async transition (indicated by an ASYNC return
 value from leaveState)
var fsm = this;
this.transition = function() {
  fsm.transition = null; // this method should only ever be called once
  fsm.current = to;
  StateMachine.enterState( fsm, name, from, to, args);
  StateMachine.changeState(fsm, name, from, to, args);
  StateMachine.afterEvent( fsm, name, from, to, args);
  return StateMachine.Result.SUCCEEDED;
};
this.transition.cancel = function() { // provide a way for caller to cancel async transition if desired (issue #22)
  fsm.transition = null;
  StateMachine.afterEvent(fsm, name, from, to, args);
...
```

#### <a name="apidoc.element.javascript-state-machine.enterThisState"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>enterThisState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.enterThisState)
- description and source-code
```javascript
enterThisState = function (fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onenter'  + to]   || fsm['on' + to],   name, from
, to, args); }
```
- example usage
```shell
...
  if ((false === specific) || (false === general))
    return false;
  else if ((StateMachine.ASYNC === specific) || (StateMachine.ASYNC === general))
    return StateMachine.ASYNC;
},

enterState: function(fsm, name, from, to, args) {
  StateMachine.enterThisState(fsm, name, from, to, args);
  StateMachine.enterAnyState( fsm, name, from, to, args);
},

//===========================================================================

buildEvent: function(name, map) {
  return function() {
...
```

#### <a name="apidoc.element.javascript-state-machine.leaveAnyState"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>leaveAnyState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.leaveAnyState)
- description and source-code
```javascript
leaveAnyState = function (fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onleavestate'],                        name, from
, to, args); }
```
- example usage
```shell
...
afterEvent: function(fsm, name, from, to, args) {
  StateMachine.afterThisEvent(fsm, name, from, to, args);
  StateMachine.afterAnyEvent( fsm, name, from, to, args);
},

leaveState: function(fsm, name, from, to, args) {
  var specific = StateMachine.leaveThisState(fsm, name, from, to, args),
      general  = StateMachine.leaveAnyState( fsm, name, from, to, args);
  if ((false === specific) || (false === general))
    return false;
  else if ((StateMachine.ASYNC === specific) || (StateMachine.ASYNC === general))
    return StateMachine.ASYNC;
},

enterState: function(fsm, name, from, to, args) {
...
```

#### <a name="apidoc.element.javascript-state-machine.leaveState"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>leaveState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.leaveState)
- description and source-code
```javascript
leaveState = function (fsm, name, from, to, args) {
  var specific = StateMachine.leaveThisState(fsm, name, from, to, args),
      general  = StateMachine.leaveAnyState( fsm, name, from, to, args);
  if ((false === specific) || (false === general))
    return false;
  else if ((StateMachine.ASYNC === specific) || (StateMachine.ASYNC === general))
    return StateMachine.ASYNC;
}
```
- example usage
```shell
...
  return StateMachine.Result.SUCCEEDED;
};
this.transition.cancel = function() { // provide a way for caller to cancel async transition if desired (issue #22)
  fsm.transition = null;
  StateMachine.afterEvent(fsm, name, from, to, args);
}

var leave = StateMachine.leaveState(this, name, from, to, args);
if (false === leave) {
  this.transition = null;
  return StateMachine.Result.CANCELLED;
}
else if (StateMachine.ASYNC === leave) {
  return StateMachine.Result.PENDING;
}
...
```

#### <a name="apidoc.element.javascript-state-machine.leaveThisState"></a>[function <span class="apidocSignatureSpan">javascript-state-machine.</span>leaveThisState (fsm, name, from, to, args)](#apidoc.element.javascript-state-machine.leaveThisState)
- description and source-code
```javascript
leaveThisState = function (fsm, name, from, to, args) { return StateMachine.doCallback(fsm, fsm['onleave'  + from],                     name, from
, to, args); }
```
- example usage
```shell
...

afterEvent: function(fsm, name, from, to, args) {
  StateMachine.afterThisEvent(fsm, name, from, to, args);
  StateMachine.afterAnyEvent( fsm, name, from, to, args);
},

leaveState: function(fsm, name, from, to, args) {
  var specific = StateMachine.leaveThisState(fsm, name, from, to, args),
      general  = StateMachine.leaveAnyState( fsm, name, from, to, args);
  if ((false === specific) || (false === general))
    return false;
  else if ((StateMachine.ASYNC === specific) || (StateMachine.ASYNC === general))
    return StateMachine.ASYNC;
},
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
