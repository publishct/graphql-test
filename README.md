# GraphQl Test

GraphQL Test is a repository based on LinkedIn Learning's intermediate course "GraphQL Essential Training" taught by Emmanuel Henri

## Description Summary

GraphQL—a query language for APIs that was originally built by Facebook—makes it easier for you to get the data you actually need from a query. In this course, learn how to get started with GraphQL. Instructor Emmanuel Henri walks through how to set up GraphQL, explores the GraphQL schema, and goes over the basic types and fields. He also shows how to set up persistence—including how to use SQL and MongoDB with GraphQL; covers how to add new items with mutations; and shares how to leverage some advanced features in your queries.

### Modifications by Cynthia Trujillo 

schema.js
```
enum Gender {
    MALE
    FEMALE
    NONBINARY
    GENDEREXPANSIVE
    GENDERLESS
    TWOSPIRIT
    GENDERNONCONFORMING
    OTHER
}
```

### Deprecation Mods 
dbConnectors.js deprecation update via Mongoose 
Documentation available at https://mongoosejs.com/docs/deprecations.html#findandmodify
```
mongoose.connect(uri, { useFindAndModify: false });
```

resolvers.js deprecation update 
Use deleteOne() instead of collection.remove
```
collection.deleteOne()
```


#### Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
