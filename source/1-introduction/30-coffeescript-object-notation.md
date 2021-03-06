# CoffeeScript Object Notation

Atom uses a configuration format called "CSON" for all of its configuration files. While [it is possible to use JSON instead][json-instead], getting used to CSON is pretty easy and I think that CSON is a better file format for configuration files than JSON is due to its simplicity. (It has a lot in common with [YAML][yaml], another common configuration file format.)

CSON is short for CoffeeScript Object Notation. It works identically to the more common [JSON][json]. As a matter of fact, almost all JSON is valid CSON. But, CSON can be written more easily and compact if certain conventions are followed. If you indent the CSON in a typical way, you are allowed to omit the curly braces (`{` and `}`) and commas (`,`). For example, this JSON:

```json
{
  "foo": 5,
  "bar": {
    "baz": false
  }
}
```

Is completely equivalent to this CSON:

```coffeescript
"foo": 5
"bar":
  "baz": false
```

Notice the only changes were to remove the curly braces, the comma and reduce the indentation by one level (because the outermost object declaration is assumed).

[json]: http://json.org/
[json-instead]: /appendices/using-javascript-and-json.html
[yaml]: http://www.yaml.org/
