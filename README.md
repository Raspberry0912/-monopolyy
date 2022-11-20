# -monopolyy
const monopoly = require("discord-monopoly");
const Discord = require("discord.js");
const bot = new Discord.Client();
const MonopolyRunner =  new monopoly({
  // config settings go here 
});

bot.on("message", (message) => {
   // whatever you're doing
   MonopolyRunner(message);
});

bot.login(/* your bot token */);
