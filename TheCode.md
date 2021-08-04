Use repl.it for the coding then download in repl.it Express, and Discord.js for the bot to work

DO NOT DELETE THESE CODE UNLESS YOU KNOW WHAT YOUR DOING RIGHT THERE!

Code :

const express = require("express")
const app = express()

app.get("/", (req, res) => {
  res.send("The bot is online on discord. please check")
})

app.listen(3000, () => {
  console.log("Bot has been online")
})
let Discord = require("discord.js")
let client = new Discord.Client()
"down here is a message, copy and paste it if you want to make the bot send a message"
client.on("message", message => {
if(message.content === "This is the prefix, edit this text for set the prefix, ") {  
  message.channel.send("This is the message")
}
  if(message.content === "!") {
  let embed = new Discord.MessageEmbed()
  .setTitle("This is the Name of your embed")
  .setDescription("This is the message")
  .setColor("RANDOM")  <---- "this is the color for your embed"
  .setFooter("This is the Small text")
  message.channel.send(embed) 

}
})

client.login("Your Bot Token");
