# MongoDB

MongoDB is a document oriented database. It is relatively easy to use because you interact with the db in much the same way you code.


### Installation Notes

Installing on Windows puts the default db folder in the same folder where the product is installed. You may want to create a db folder somewhere else. But then you will need to start the MongoDB server in a different way than autostart as a service so you can speficy the new folder as the startup db folder.

Use the following command to start the MongoDB server and specify the db path. Fill in the actual path on your machine.

`>mongod --dbpath "<PATH>\db"`


