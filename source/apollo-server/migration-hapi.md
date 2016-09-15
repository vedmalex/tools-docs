---
title: Migrating from v0.2
order: 206
description: How to migrate from an older version of Apollo Server
---

Version 0.3.0 of Apollo Server contains a couple of breaking changes in the Hapi plugin API.
The most notable changes are:

- the plugin class has been replaced as a function to be more idiomatic
- the plugin name has been renamed to use camelcase
- the options object has been extended to support additional routing options

The following code snippet for Hapi Apollo 0.2.x

```js
import { ApolloHAPI } from 'apollo-server';
...
server.register({
    register: new ApolloHAPI(),
    options: { schema: myGraphQLSchema },
    routes: { prefix: '/graphql' },
});
```

... should be written as follows for Hapi Apollo 0.3.x

```js
import { ApolloHapi } from 'apollo-server';
...
server.register({
    register: ApolloHapi,
    options: {
      path: '/graphql',
      apolloOptions: {
        schema: myGraphQLSchema,
      },
      route: {
        cors: true
      }
    },
});
```

*NOTE:* That you can now pass additional routing configuration via the route options
