- The graph is deployed to https://thegraph.com/hosted-service/subgraph/haowang1013/graph-test

- It's now indexing the BYAC contract and before the indexing is done, you can access the pending version here: https://api.thegraph.com/subgraphs/id/QmZcEF5HAGU1maRMSQTGgAUxxrugiw9taSY7qfwe84HesE

- A simple query that shows the `from` field is missing from the transfer event:
```
{
  erc721Contracts {
    id
    transfers(first: 10) {
      transaction {
        id
      }
      from {
        id
      }
    }
  }
}
```
