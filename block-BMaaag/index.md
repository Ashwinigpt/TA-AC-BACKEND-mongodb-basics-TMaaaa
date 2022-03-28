writeCode

Write code to:-

- create a database named `mountains`
use mountains

- a collection inside that database named `himalayas`
db.createCollection('himalyas');

- insert 1 document into that collection `{name: 'Dhauldhar range', height: '4000 mtrs'}`
db.himalyas.insert({name: 'Dhauldhar range', height: '4000 mtrs'});

- insert multiple document using insertMany command
db.himalyas.insertMany([{
    name: 'Dhauldhar range', 
    height: '4000 mtrs
  },
  {
    name: 'Dhauldhar range', 
    height: '4000 mtrs
  },
  {
    name: 'Dhauldhar range', 
    height: '4000 mtrs
  },
  {
    name: 'Dhauldhar range', 
    height: '4000 mtrs
  },
])

- find all documents from mountains
db.mountains.find();

- find a single document using name
db.mountains.findOne({name: 'Dhauldhar range'});