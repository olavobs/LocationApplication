# LocationApplication
Location Application using Springboot and h2 database with JPA based on Java Developer Nanodegree from Udacity for understand GraphQL.


## Start Application: 

- Application will run on port 8080

### Access h2 console: 

```
localhost:8080/h2
```

### Access graphiql
```
http://localhost:8080/graphiql
```


### Endpoints:
 - Query: 
  ```
 {
   findAllLocations {
    id
    address
    name
   }
}
```
  
 - Mutation:
  
  1) deleteLocation: 
  ```
  mutation {
    deleteLocation(id: ID!): Location!
  }
  ```
  2) updateLocationName:
  ```
  mutation {
   updateLocationName(newName: String!, id: ID!){
    id
    name
    address
   }
 }
  ```
  
 3) newLocation:
 ```
  mutation {
   newLocation(
    name: String!,
    address: String!) {
   	id
    name
    address
   }
 }
 ```
