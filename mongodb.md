# MongoDB

MongoDB is a document oriented database. It is relatively easy to use because you interact with the db in much the same way you code.


### Startup Notes

Installing on Windows puts the default db folder in the same folder where the product is installed. You may want to create a db folder somewhere else. But then you will need to start the MongoDB server in a different way than autostart as a service so you can speficy the new folder as the startup db folder.

In a Windows command prompt, run `NET START` to see what services are running. If you see **MongoDB Server** then you need to stop it and you may want to update the Startup Type to **Manual** instead of **Automatic**. To do that type `Services` in the Windows search box. Scoll to **MongoDB Server** and update the properties.

Once you have stopped the auto start service. Use the following command to start the MongoDB server and specify the db path. Fill in the actual path on your machine.

`mongod --dbpath "<PATH>\db"`


### Basic Commands

`show dbs` Three default dbs will show up.

`use store` This chooses the active database. If **store** is not there it will be created.

`db.product` The text **db** refers to the active database. Currently this is **store**. The text **product** refers to a Collection. If **product** is not there it will be created.

`db.product.insertOne({name: "Airsoft Electric Rifle", price: 159.99})` This inserts a document in the **product** collection.

`db.product.find()` This will list all the documents in the collection.

`db.product.find().pretty()` This formats the output a little more readable.



