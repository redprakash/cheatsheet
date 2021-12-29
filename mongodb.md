# List of useful MondoDb Commands
### View all databases
```show dbs```

### Create a new database or switch database
```use yourDatbaseName```

### View the current database you are on
```db```

### Delete Database
```db.dropDatabase()```

## Working with Collections
- A collection is a grouping of MongoDB documents. Documents within a collection can have different fields. 
- A collection is the equivalent of a table in a relational database system. 
- A collection exists within a single database

### View Collections
```show collections```

### Create new collection
```db.createCollection('nameOfCollection')```

### Delete a collection
```db.nameOfCollection.drop()```

## Working with Documents
### View all documents in a Collection
```db.nameOfCollection.find()```

### View in organised or pretty way
```db.nameOfCollection.find().pretty()```

## Reading Documents
### Find the first matching document in a collection
```db.nameOfCollection.find({key:value})```
- Example, Find the document whose name is 'Prakash'
  - ```db.nameOfCollection.find({name:'Prakash'})```
 
 ### Less than -> $lt, less than or equal -> $lte
 ### Greater than -> $gt, greater than or equal -> $gte
 #### Find those, whose prices are less than or equal to 300
 ```db.nameOfCollection.find({ price: {$lte:300 } })```
 #### Searching with
 
 
