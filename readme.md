# Preeti translation

###### add preeti.js

```javascript
// <input type="text" class="convert-preeti">
$("body").on("input", ".convert-preeti", function (event) {
  var text = this.value;
  var convert = setUnicodePreeti(text);
  this.value = convert;

  return true;
});
// Example: sf]bh]g = कोदजेन
```

# Romanize translation

###### add romanize.js

```javascript
// <input type="text" class="convert-romanize">
$("body").on("keypress", ".convert-romanize", function (event) {
  return setUnicode(event, this);
});
// Example: kodejen = कोदजेन
```
