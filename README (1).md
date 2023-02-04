# README

### Prisma Client Go

#### Typesafe database access for Go

[![](https://img.shields.io/github/v/release/prisma/prisma-client-go)](https://github.com/prisma/prisma-client-go/releases)    [![](https://github.com/prisma/prisma-client-go/actions/workflows/test.yml/badge.svg)](https://github.com/prisma/prisma-client-go/actions/workflows/test.yml)    [![](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](<README (1).md#contributing>)    [![](https://img.shields.io/github/license/prisma/prisma-client-go)](LICENSE/)    [![](https://img.shields.io/badge/chat-on%20slack-blue.svg)](https://slack.prisma.io/)[Quickstart](docs/quickstart.md)   •   [Website](https://www.prisma.io/)   •   [Docs](docs/)   •   [API reference](docs/reference/)   •   [Blog](https://www.prisma.io/blog)   •   [Slack](https://slack.prisma.io/)   •   [Twitter](https://twitter.com/prisma)

***

### Deprecation note

**Prisma Client Go is no longer officially maintained**. Read [this issue](https://github.com/prisma/prisma-client-go/issues/707) to learn more.

### Description

Prisma Client Go is an **auto-generated query builder** that enables **type-safe** database access and **reduces boilerplate**. You can use it as an alternative to traditional ORMs such as gorm, xorm, sqlboiler and most database-specific tools.

It is part of the [Prisma](https://www.prisma.io/) ecosystem. Prisma provides database tools for data access, declarative data modeling, schema migrations and visual data management.

_NOTE_: Prisma Client Go is currently offered under our [early access program](https://www.prisma.io/docs/about/releases#product-maturity-levels). There will be documented breaking changes with new [releases](https://github.com/prisma/prisma-client-go/releases).

### Getting started

To get started, [**read our quickstart tutorial**](docs/quickstart.md) to add Prisma to your project in just a few minutes.

You also might want to read [deployment tips](docs/deploy.md) and the [full API reference](docs/reference/).

### Notes

The go client works slightly different than the normal Prisma tooling. When you're using the go client, whenever you see Prisma CLI commands such as `prisma ...`, you should always write `go run github.com/prisma/prisma-client-go ...` instead.

If you just work with the Go client and don't have (or want) the NodeJS Prisma CLI installed, you can set up an alias so that you can write `prisma` commands as usual, but it'll invoke the real locally bundled Prisma CLI. To do that, edit your `~/.bashrc` or `~/.zshrc` and add:

```
alias prisma="go run github.com/prisma/prisma-client-go"
```

Now `prisma generate` and any other command will work, and it'll just run 1`go run github.com/prisma/prisma-client-go generate` under the hood.

### Contributing

Check out our [advanced contributing guide](./).

### Security

If you have a security issue to report, please contact us at [security@prisma.io](mailto:security@prisma.io?subject=\[GitHub]%20Prisma%202%20Security%20Report%20Go)
