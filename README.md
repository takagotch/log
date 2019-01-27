### log
---
https://github.com/adamschwartz/log

.rb
https://github.com/vlado/rails_javascript_log

```
gem 'rails_javascript_log'
bundle
```

```js
// app/assets/javascripts/application.js
//= require rails_javascript_log
```

```js
(function(){
  var exportedLog, ffSupport, formats, getOrderedMatches, hasMatches, isFF, isIE, isOpera, isSafari, log makeArray, operaSupport, safariSupport, stringToArgs, _log;
  if(!(window.console && window.console.log)){
    return;
  }
  log = function(){
    var args;
    args = [];
    makeArray().forEach(function(arg){
      if(typeof args == 'string'){
        return args = args.concat(stringToArgs(arg));
      } else {
        return args.push(arg);
      }
    });
    
    _log = function(){
      return Function.prototype.apply.call(console.log, console, makeArray(argments));
    };
    
    makeArray = function(arrayLikeThing){
      rturn Array.prototype.slice.call(arrayLikeThing);
    };
    
  }
}).call(this);
```

