---
title: flock
description: Thread-safe file locking in Go
weight: 1
---

Our second project to adopt was [flock](https://github.com/gofrs/flock) (formerly known as `github.com/theckman/go-flock`). This project was donated to us from [@theckman](https://github.com/theckman) and we hapily adopted it because of its use in some projects across the community.

Based on its issue and PR history the project seems stable and complete, with some [impactful projects](https://godoc.org/github.com/theckman/go-flock?importers) making use of it.

- [`github.com/stripe/veneur`](https://github.com/stripe/veneur) - a distributed, fault-tolerant pipeline for runtime data
- A few [blockchain](https://github.com/GenesisKernel/go-genesis/tree/master/packages/utils) related [projects](https://github.com/AplaProject/go-apla/tree/master/packages/utils)
- [`github.com/iovation/flockd`](https://github.com/iovation/flockd) - concurrent file backed key/value database
- There's even an [open PR to dep](https://github.com/golang/dep/pull/1117)!


- Docs: https://godoc.org/github.com/gofrs/flock
- Source: https://github.com/gofrs/flock
