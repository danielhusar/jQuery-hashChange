jQuery hash change plugin
======================================

Fire all callbacks when hash change.

Sample usage
============

With addHashCallback helper.
```javascript
	var a = function(hash){console.log(hash)};
  var b = function(hash){console.log(hash + hash)};
  $.addHashCallback(a);
  $.addHashCallback(b);
	$.hashChange();
```

Passing array of callbacks;
```javascript
	var a = function(hash){console.log(hash)};
  var b = function(hash){console.log(hash + hash)};
  var arr = new Array();
  arr.push(a);
  arr.push(b);
	$.hashChange(arr);
```

Passing directly a callback;
```javascript
	$.hashChange(function(hash){
		console.log(hash);
	});
```

See demo section for demo.