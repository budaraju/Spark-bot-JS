## Checklist (absolute bare minimum to get a helloworld bot working)

Prerequisites:
node.js (minimum supported v4.2.6 with *use-strict* runtime flag & npm 2.14.12 and up)

Sign up for Cisco Spark (logged in with your web browser)

----

Create a Cisco Spark Bot (save the API key): https://developer.ciscospark.com/add-bot.html

Sign up for nGrok (save API key) and start it on your machine (save the port number and public web address): https://ngrok.com/download

Join a room in Cisco Spark

Add the bot to the room in Spark

Obtain the roomId from an authenticated GET using the Cisco Spark API: https://developer.ciscospark.com/endpoint-rooms-get.html

Create a webhook with the roomId and using your nGrok address, roomId, by POSTing to Cisco Spark API: https://developer.ciscospark.com/endpoint-webhooks-post.html

Add the port/nGrok address and API bot key to your bot server config.json

Turn on your bot server with ```npm start```

