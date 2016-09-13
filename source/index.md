---
title: Introduction
order: 0
---

In addition to a set of fully-featured GraphQL clients, the Apollo community maintains a set of tools for building GraphQL servers and clients.

### GraphQL server tools

- [Apollo Server](/tools/apollo-server), a production-ready Node.js GraphQL server library that supports Express, Connect, Hapi, Koa, and other popular Node HTTP servers, with built-in features like persisted queries, batching, and more. Apollo Server works with any GraphQL client, like Apollo, Relay, Lokka, and more.
- [graphql-tools](/tools/graphql-tools), a package that provides an alternative approach to constructing a GraphQL.js schema using the GraphQL schema language, rather than using the GraphQL.js type constructors directly. Schemas built with this package are compatible with any GraphQL servers, including our own `apollo-server` and Facebook's `express-graphql`.
- Todo: add subscriptions server here

### GraphQL client tools

- [graphql-anywhere](https://github.com/apollostack/graphql-anywhere), the core schema-less GraphQL execution engine of the Apollo JavaScript Client, which lets you build your own powerful GraphQL tools and cache implementations, and works anywhere you can run JavaScript code.
- Todo: add subscriptions client here

### Developer tools

- [eslint-plugin-grapql](https://github.com/apollostack/eslint-plugin-graphql), an ESLint plugin that will check your GraphQL query strings for syntax errors and schema compliance, and works with any JavaScript GraphQL client including Apollo, Relay, Lokka, and more.
