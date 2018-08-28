---
title: uuid
description: The package that served as the catalyst for the Gofrs forming. This is a fork of the github.com/satori/go.uuid package. This package was forked after it appeared to be no longer maintained, while having critical bugs that made it unsafe for use in some cases.
weight: 1
---

The first project we adopted, which happened to be the catalyst for the group
forming, was the [UUID](https://github.com/gofrs/uuid) package, which was forked
from [github.com/satori/go.uuid](https://github.com/satori/go.uuid). The
`go.uuid` package one likely the most used UUID package in the Go ecosystem, but
had recently introduced [breaking API changes without a release](https://github.com/satori/go.uuid/issues/66),
as well as critical bugs rendering the UUIDs generated [not being guaranteed to
be unique](https://github.com/satori/go.uuid/issues/73).

The initial release we cut was `v2.0.0`, which retained API compatibility with
the `master` branch of `satori/go.uuid`. Because the Gofrs adhere to the
Semantic Versioning v2.0.0 standard, the entire `v2.x` series is API compatible.

The `v3.0.0` release was made after changes were made to how the `NullUUID` type
would render JSON, and the removal of the `Equal()` package function. At this
time we do not anticipate further breaking changes.

- Source: https://github.com/gofrs/uuid
- Docs: https://godoc.org/github.com/gofrs/uuid
