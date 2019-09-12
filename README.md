# Inquery-Local
Monitor your GraphQL endpoint.

Note: This module is for testing your GraphQL endpoint on your local machine. 

Step 1. 
```npm install inquery-monitor-local```

Step 2. 
```const { enableMonitoring } = require('inquery-monitor-local```

Step 3.
Pass your resolvers in as the first param to enableMonitoring.

```
const updatedResolvers = enableMonitoring(oldResolvers)
```

Step 4.
Start your server with updated resolvers.
```
const server = new ApolloServer({ typeDefs, updatedResolvers })

server.listen( ).then( { url } ) ⇒ { console.log(`Server is listening at { url }` )}) 
```

Step 5.
Run in your terminal the following command. 
```
inquery monitor
```

