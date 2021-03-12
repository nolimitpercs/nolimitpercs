const app = express()

app.get("/", (req, res) => {
 res.send("Server Mod bot")
})

app.listen(3000, () => {
 console.log("Whatever you want to put here")
})

let Discord = require("discord.js");
let client = new Discord.Client();
client.on("message", message => {
if (message.content === "hello") {
message.channel.send("hii!!")

if(message.content === "-help") {
 let embed = new Discord.MessageEmbed()
 .setTitle("Help")
 .setDescription("Hello there. go read https://bit.ly/3tezdCi")
 .setFooter(" tbh nothing here tho")
 message.channel.send(embed)
 }
if(message.content === "-info") {
 let embed = new Discord.MessageEmbed()
 .setTitle("i an server mod bot")
 .setDescription("so i was created by this 13 y/o called ! nelly")
 .setColor("PURPLE")
 .setFooter("theres more coming")
 message.channel.send(embed)
}

if(message.content === ("testbot") {
  message.channel.send("Is working")
} 

}
})


client.login("ODIwMDIwNDA2MDE0MzEyNTE4.YEvFhA.jnGRHZdHf3ECVpdVzgwdDm4SHbA") 
