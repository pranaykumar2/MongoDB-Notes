# Day 1 - MongoDB

A document database designed for ease of application development and scaling.

## What We Can Do with Data in MongoDB

- Store and query the data
- Transform data with aggregations
- Secure access to your data
- Deploy and scale your database

## MongoDB Documents

A record in MongoDB is a document (specifically BSON documents), and a document consists of fields of key-value pairs (JSON objects). Values may include other documents, arrays, or arrays of documents.

### Example: Inserting a Document

Created using `db.student.insertOne()`:

```javascript
db.student.insertOne({
  name: "pranay",
  age: 12,
  blood: "o+",
  hobbies: ["Listening Music", "Reading"]
});
```

Upon successful insertion, the operation returns a document that contains the acknowledgement indicator and an array that contains the `_id` of each successfully inserted document:

```javascript
{
  acknowledged: true,
  insertedId: ObjectId('6856eff54b33c7573550eb67')
}
```

### Advantages

- Documents correspond to native data types
- Reduce need for expensive joins
- Dynamic schema supports fluent polymorphism

## MongoDB Collections

MongoDB stores documents in a collection. A collection is equivalent to a table in SQL.

**Note:** If a collection does not exist, MongoDB creates the collection when you first store data for that collection.

## Key Features

- **High Performance**
- **Query API** (CRUD, Data aggregation, text search, and geo-spatial queries)
- **High Availability** (replica set)
- **Horizontal Scalability** (sharding, zones)
- **Support for Multiple Storage Engines**

---

### Upcoming

**Day 2** - Complete Databases and Collections in MongoDB
