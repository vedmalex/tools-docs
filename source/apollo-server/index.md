---
title: Installing
order: 201
description: How to install Apollo Server
---

Apollo Server is a community driven, flexible, production-ready HTTP JavaScript GraphQL server. It works with any GraphQL schema built with GraphQL.js, Facebook's reference JavaScript execution library. You can also use the [graphql-tools](/tools/graphql-tools) package to generate those schema objects from schema language strings.

You can use Apollo Server with all popular JavaScript web servers, including Express, Connect, Hapi, and Koa.

Install it with:

```txt
npm install apollo-server
```

The following features distinguish Apollo Server from [express-graphql](https://github.com/graphql/express-graphql), Facebook's reference HTTP server implementation:

- Apollo Server has a simpler interface and allows only one way of sending queries--POST requests--which makes it a bit easier to reason about what's going on.
- Apollo Server serves GraphiQL on a separate route, giving you more flexibility to decide when and how to serve it.
- Apollo Server supports [query batching](https://medium.com/apollo-stack/query-batching-in-apollo-63acfd859862) which can help reduce load on your server.
- Apollo Server has built-in support for query whitelisting, which can make your app faster and your server more secure.
