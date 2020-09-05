# Free Frames
 FreeFrames is to add some frames to your picture or to make some memes
 
 # Toggle Links
 
 - ****[Installation](#Installation)****
 - ****[Example Codes For Discord.JS](#Example)****
 
 ## Installation
 `npm install freeframes --save`
 
 ## Example Discord.js
 ```
 const discord = require('discord.js');
 const client = new discord.Client();
 const frames = require('freeframes');
 let prefix = '!';
 
 client.on('ready', () => {
  console.log('ready!');
 });
 
 client.on('message', async message => {
  if(message.content.startsWith(prefix + 'image')){
    let image = await frames.Image(your avatar);
    let png = new discord.MessageAttachment(image, 'image.png');
    message.channel.send(png);
 });
 
 clint.login('XXXXXX');
 ```
 
 
