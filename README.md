# noisechatter
![nb_logo](https://user-images.githubusercontent.com/105610230/169454383-14ca67c5-ecf4-45f3-ac23-1a966a4a4699.png)

Noisechatter is an extension of the Noisebridge BBS. It's meant to complement other features of the BBS by providing a sidechannel for chatters using a Javascript web application using Node.js and Socket.io.

This repo uses James Q. Quick's code from his 8 part tutorial, "Design and Build a Chat App with Socket.io." The link to the playlist is <a href="http://iteroni.com/playlist?list=PLDlWc9AfQBfbyGwhSlxg16mQGpGnauCwq" target=_blank> here.</a> This is a great series and I highly recommend it.

# Demo
See noisechatter in action by visiting my instance of it at this <a href="http://possessed.duckdns.org:3000" target=_blank>link</a>.

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

Once you've cloned the repo, you'll need to deploy the server.js file located in the top folder. To accomplish this, you will need PM2 installed. There are multiple ways to deploy an app, but I assure you none are as easy as PM2.

Run the following command from the top folder, which contains the server.js file:

`pm2 start server.js` 

The default port is :3000. It will look something like this when you provide a link to your instance.

YOURIP:3000 or YOURDOMAIN:3000

I use duckdns as a way to provide a quick and operational domain for this app. You can do the same by visiting <a href="https://www.duckdns.org/" target=_blank>duckdns.org</a>

# Known Issues and Limitations

- If you close your chat session all your cannot be recovered.
- No alerting method when you receive a message
- No HTTPS by default. If you want this you need a cert. Look into a certificate using <a href="https://letsencrypt.org/" target=_blank>Let's Encrypt.</a>
- No persistent usernames. Signing in with the same name just creates a duplicate name.
- If you press a key and hold it down with no spaces involved it will trail off the screen like so. AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA. Try it for fun.
- No password protection.
- No encryption.
- No DMs or multiple rooms to choose from.

This should get you started. This is just a basic Node.js app with standard HTML, CSS, and Javascript files. It would be trivial to customize the look and feel on your own.

# Future Features

- ANSI ART
- Rooms
- DMs
- Security stuff

# Check out Noisebridge online or visit us at 272 Capp St. in San Francisco, CA!

Check out our projects at www.noisebridge.net! 
![Noisebridge-pixels](https://user-images.githubusercontent.com/105610230/169455517-3732a8cf-9d82-4d45-81e9-52d6f6ad1873.gif)

-  Join the Noisebridge BBS at <a href="possessed.duckdns.org/vtx.html" target=_blank> this link via websockets!</a>
-  Using a terminal client like Netrunner, connect with us at possessed.duckdns.org:8888 via telnet.
-  Also, checkout our Moebius server at possessed.duckdns.org:8000 where you can draw ANSI art with us!
-  Detailed connection instructions for our BBS are located on our main page wiki under the BBS channel.

