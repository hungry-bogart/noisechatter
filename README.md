# noisechatter
![nb_logo](https://user-images.githubusercontent.com/105610230/169454383-14ca67c5-ecf4-45f3-ac23-1a966a4a4699.png)

Noisechatter started as an extension of the Noisebridge BBS. It was meant to complement other features of the BBS by providing a sidechannel for chatters using a Javascript web application built with Node.js and Socket.io. Sadly, it was never used to its full potential and the Noisebridge BBS is on hiatus.

# Inspiration

This repo uses James Q. Quick's code from his 8 part tutorial, "Design and Build a Chat App with Socket.io." The link to the playlist is <a href="http://iteroni.com/playlist?list=PLDlWc9AfQBfbyGwhSlxg16mQGpGnauCwq" target=_blank> here.</a> This is a great series and I highly recommend it.

# Dependencies

PM2
https://github.com/Unitech/pm2

NodeJS and Node Package Manager(NPM)
https://docs.npmjs.com/downloading-and-installing-node-js-and-npm

Node Modules Used:

http, express, socket.io, and path. If you get lost at any point in time, watch the playlist at the top of this README.md file.

Links to the main modules are below.

https://socket.io/

https://expressjs.com/


# Installation

`git clone https://github.com/hungry-bogart/noisechatter`

Once you've cloned the repo, you'll need to deploy the server.js file located in the top folder. You have two options. For the first option, you will need PM2 installed. I assure you, there are many ways to deploy an app, but none are as easy as PM2.

Run the following command from the top folder, which contains the server.js file:

`pm2 start server.js` 

The default port is :3000. It will look something like this when you provide a link to your instance.

YOURIP:3000 or YOURDOMAIN:3000

I use duckdns as a way to provide a quick and operational domain for this app. You can do the same by visiting <a href="https://www.duckdns.org/" target=_blank>duckdns.org</a>

If you simply want to test the app, or you don't want to install pm2, type this in your terminal instead.

`node server.js`

# Coming Soon Docker Version
I'm still working on this, but I wanted to check the code and redo the UI a bit before I push it to the repo here.

# Known Issues and Limitations

- If you close your chat session, your messages cannot be recovered.
- No alerts when you receive a message if you are away.
- No HTTPS by default. If you want this feature, you need a cert. Look into a certificate using <a href="https://letsencrypt.org/" target=_blank>Let's Encrypt.</a>
- No persistent usernames. Signing in with the same name just creates a duplicate name.
- If you press a key and hold it down with no spaces involved it will trail off the screen. Like this: AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA. Try it for fun.
- No password protection.
- No encryption.
- No DMs or multiple rooms to choose from.

This should get you started. This is just a basic Node.js app with standard HTML, CSS, and Javascript files. It would be trivial to customize the look and feel on your own.

# Future Features
- ANSI ART
- Rooms
- DMs
- Security stuff
- More security stuff...

# Check out Noisebridge online or visit us at 272 Capp St. in San Francisco, CA!

Check out our projects at www.noisebridge.net! 

![Noisebridge-pixels](https://user-images.githubusercontent.com/105610230/169455517-3732a8cf-9d82-4d45-81e9-52d6f6ad1873.gif)

