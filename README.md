# alumbra.spec

This library contains [clojure.spec][cljspec] specifications for the data
structures used in alumbra's GraphQL parsing, validation and execution. Its goal
is a clear description of the interfaces between the different GraphQL
components to allow for pluggable implementations.

[![Build Status](https://travis-ci.org/alumbra/alumbra.spec.svg?branch=master)](https://travis-ci.org/alumbra/alumbra.spec)
[![Clojars Project](https://img.shields.io/clojars/v/alumbra/spec.svg)](https://clojars.org/alumbra/spec)

[cljspec]: http://clojure.org/guides/spec

## Usage

```clojure
(require 'alumbra.spec)
```

## Available Specs

__`:alumbra/document`__

Describes the AST of a GraphQL document.

__`:alumbra/schema`__

Describes the AST of a GraphQL schema.

__`:alumbra/canonical-operation`__

Describes a canonical, self-contained format for a GraphQL operation that
can be interpreted without further knowledge of the GraphQL schema.

__`:alumbra/analyzed-schema`__

An analyzed version of a GraphQL schema, removing AST-specific information like
metadata and providing inline maps where appropriate.

__`:alumbra/parser-errors`__

Describes a seq of parser errors for a given GraphQL schema or query document.

__`:alumbra/validation-errors`__

Describes a seq of validation errors for a given GraphQL schema and query
document.

## License

```
MIT License

Copyright (c) 2016-2017 Yannick Scherer

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
