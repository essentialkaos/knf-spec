## KNF File Format Specification

This document specifies `knf` file format also known as _KNF configuration file_.

### Syntax

#### Properties

The essential element contained in a KNF file is _property_. Every property has a name and a value, delimited by a colon sign (`:`). The name appears to the left of the colon sign.

```
name: value
```
Double or single quotes can surround string values. These strings MUST be removed in the process of parsing and MUST NOT be a part of the value.

```
name: "Text value"
```

### License

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)

<p align="center"><a href="https://essentialkaos.com"><img src="https://gh.kaos.st/ekgh.svg"/></a></p>
