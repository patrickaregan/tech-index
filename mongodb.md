# MongoDB

MongoDB is a document oriented database. It is relatively easy to use because you interact with the db in much the same way you code.


### Startup Notes

Installing on Windows puts the default db folder in the same folder where the product is installed. You may want to create a db folder somewhere else. But then you will need to start the MongoDB server in a different way than autostart as a service so you can speficy the new folder as the startup db folder.

In a Windows command prompt, run `NET START` to see what services are running. If you see `MongoDB Server` then you need to stop it and you may want to update the Startup Type to **Manual** instead of **Automatic**. To do that type `Services` in the Windows search box. Scoll to **MonboDB Server** and update the properties.

Once you have stopped the auto start service. Use the following command to start the MongoDB server and specify the db path. Fill in the actual path on your machine.

`>mongod --dbpath "<PATH>\db"`



