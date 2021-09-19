## KNF File Format Specification

This document specifies `knf` file format also known as _KNF configuration file_.

### Syntax

#### Properties

The essential element contained in a KNF file is _property_. Every property has a name and a value, delimited by a colon sign (`:`). The name appears to the left of the colon sign.

```
name: value
```

#### Sections 

Properties MUST be grouped into arbitrarily named _sections_. The section name appears on a line by itself, in square brackets (`[` and `]`). All properties after the section declaration are associated with that section. There is no explicit "end of section" delimiter; sections end at the next section declaration or at the end of the file. Sections CANNOT be nested.

Properties may, but need not, have a whitespace or tab indentation.

```
[section]
  a: 1
  b: 2
```

#### Case sensitivity

Section and property names ARE NOT case sensitive.

#### Comments

Number sign (`#`) at the beginning of the line indicate a comment. Comment lines are ignored.

#### Duplicate names

Duplicate names of sections or properties within one section ARE NOT allowed.

### License

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)

<p align="center"><a href="https://essentialkaos.com"><img src="https://gh.kaos.st/ekgh.svg"/></a></p>
