writeCode

Write code to:-

- create a database named `sports`.
use sports

- list all databases present in local mongod server.
show dbs

- create 3 collections named `cricket`, `football`, `TT` in sports databse.
db.createCollection('cricket', 'football', 'TT');

- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
db.cricket.insert([{name: 'Ashwini'}, {age: 23}, {email: 'ashwinigpt1996@gmail.com'}, {bid_price: 25$}]);
db.football.insert([{name: 'Ashwini'}, {age: 23}, {email: 'ashwinigpt1996@gmail.com'}, {bid_price: 25$}]);
db.TT.insert([{name: 'Ashwini'}, {age: 23}, {email: 'ashwinigpt1996@gmail.com'}, {bid_price: 25$}]);

- list all collections in sports database.
show collections

- rename `TT` collection to `tennis`.
TT.rename('tennis');

- create a capped collection called `khokho` which should have max 3 documents.
db.createCollection('khokho', {capped: true, size: 1024, max: 3});

  Try inserting more than 3 and see what happens?
  db.khokho.insertMany([{name: 'Ashwini'}, {age: 23}, {email: 'ashwinigpt1996@gmail.com'}, {bid_price: 25$}])

- check whether a collection is capped or not?
db.khokho.isCapped();

- drop all documents from `football` collection.
db.football.find();

- delete cricket collection completely.
db.cricket.drop();

- delete sports database.
db.dropDatabase();

- check which database you are connected to ?
db

- connect to test database
use test
