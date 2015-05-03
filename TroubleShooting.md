
```
tm.timeline.layout();
```
> If no events are loaded, even though they're showing up on the map, you might be formatting your dates wrong - standard ISO8601 formatting is the best bet (e.g. "2005-05-15").

  * Be aware that trailing commas and missing semicolons in JSON declarations can throw an error in IE. So this:
```
var test = {
  title: "Test title",
  description: "A description!", // <--- problem comma
} // <--- missing semicolon
```

> needs to be this:
```
var test = {
  title: "Test title",
  description: "A description!"
};
```