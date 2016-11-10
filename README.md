# alumbra.spec

This library contains [clojure.spec][cljspec] specifications for the data
structures used in alumbra's GraphQL parsing, validation and execution. Its goal
is a clear description of the interfaces between the different GraphQL
components to allow for pluggable implementations.

[![Build Status](https://travis-ci.org/alumbra/alumbra.spec.svg?branch=master)](https://travis-ci.org/alumbra/alumbra.spec)
[![Clojars Project](https://img.shields.io/clojars/v/alumbra/spec.svg)](https://clojars.org/alumbra/spec)

[cljspec]: http://clojure.org/guides/spec

## Available Specs

__`:alumbra.spec.document/document`__

Describes the AST of a GraphQL document.

__`:alumbra.spec.schema/schema`__

Describes the AST of a GraphQL schema.

__`:alumbra.spec.canonical-document/document`__

Describes a canonical, self-contained format for a GraphQL document that
can be interpreted without further knowledge of the GraphQL schema.

__`:alumbra.spec.validator/errors`__

Describes a seq of validation errors for a given GraphQL schema and query
document.

__`:alumbra.spec.analyzer/schema`__

An analyzed version of a GraphQL schema, removing AST-specific information like
metadata and providing maps where appropriate.

## License

```
MIT License

Copyright (c) 2016 Yannick Scherer

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