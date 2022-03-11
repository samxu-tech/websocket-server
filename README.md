# Websocket client/server demo  

## Contents
Using nodejs, koa2, socket.io


## How to use it

git clone the project
enter the project root folder
npm install

npm run dev

you can visit the website in http://localhost:3001/index.html


## How to modify the client websocket connection address and port

/public/javascripts/chat.js
const socket = io('ws://localhost:3001')


## How to modify the server websocket connection port
var port = normalizePort(process.env.PORT || '3001');


## How to start the project using pm2
(1) if you want to use pm2 to manage your project , you can run:
pm2 start ./bin/www #start koa2 project

(2)pm2 restart automatically
if you want to set pm2 restart automatically  you can add the parameters:
pm2 start ./bin/www --watch