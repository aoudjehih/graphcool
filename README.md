# graphcool

1- $ npm install -g graphcool  <br/>
2- $ graphcool init  <br/>
3- graphcool local up  <br/>
4- graphcool deploy  <br/>
5- graphcool playground  <br/>
6- in opened console add user <br/>
```graphql
mutation {
  createUser(
    name: "Anis"
    dateOfBirth: "2017-09-12T00:00:00"
  ) {
    id
  }
}
```
7- we can fetch the mutated object with query <br/>
 ```graphql
query {
  allUsers(last: 1) {
    id
    name
    dateOfBirth
  }
}
 ```
to obtain:
```graphql
{
  "data": {
    "allUsers": [
      {
        "id": "ckci8o9u5003k0182uivmo9zn",
        "name": "Anis",
        "dateOfBirth": "2017-09-12T00:00:00.000Z"
      }
    ]
  }
}
```
