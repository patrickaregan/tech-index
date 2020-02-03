# MongoDB

MongoDB is a document oriented database. It is relatively easy to use because you interact with the db in much the same way you code.


### Startup Notes

Installing on Windows puts the default db folder in the same folder where the product is installed. You may want to create a db folder somewhere else. But then you will need to start the MongoDB server in a different way than autostart as a service so you can speficy the new folder as the startup db folder.

In a Windows command prompt, run `NET START` to see what services are running. If you see **MongoDB Server** then you need to stop it and you may want to update the Startup Type to **Manual** instead of **Automatic**. To do that type `Services` in the Windows search box. Scoll to **MongoDB Server** and update the properties.

Once you have stopped the auto start service. Use the following command to start the MongoDB server and specify the db path. Fill in the actual path on your machine.

`mongod --dbpath "<PATH_TO_YOUR_DB_FOLDER>\db"`

In a separate command prompt from the one you started mongod you can use mongo to connect to the server and run queries.

`mongo`


### Basic Commands

`show dbs` Three default dbs will show up.

`use store` This chooses the active database. If **store** does not exist it will be created.

`db.product` The text **db** refers to the active database. Currently this is **store**. The text **product** refers to a Collection.

`db.product.insertOne({name: "Some product name", price: 159.99})` This inserts a document in the **product** collection. If **product** does not exist it will be created.

`db.product.find()` This will list all the documents in the collection.

`db.product.find().pretty()` This formats the output a little more readable.


## Installing on Ubuntu 19.10

`sudo apt update`
`sudo apt install mongodb`
`sudo systemctl status mongodb`
It should show **active (running)**

### To Stop

`sudo systemctl stop mongodb`

### To Start

`sudo systemctl start mongodb`

### To Show Status

`sudo systemctl status mongodb`

### Run Queries

`mongo`





