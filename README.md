# Lost Kittens Discord Bot

This bot is the only one you really need for your Discord server.

It's meant to make a cat hide somewhere, in one of your Discord server's channel. The members of your community must find it by calling it. But the cat is really well hidden, so all of them must try!

Wanna try it? Join my demo Discord server! https://discord.gg/4nhqwqXP5c

## Setup the bot on your own server

[Follow this link](https://discord.com/api/oauth2/authorize?client_id=804856585582280757&scope=bot&permissions=11328) to add the bot to one of your servers.

A new game will start instantly after you add the bot to your server. Note that the game has the default configuration at this step:

- **Language**: English
- **Autorestart**: on
- **Automatically erase *Meow?* messages**: off
- The cat can hide in any of your server's channels

### Recommendations 

While this game can motivate your community, you can avoid annoying non-playing members to be spammed by *Meow?* messages with two settings:

- Specify a category which will contain the only channels where the game will happen. You can configure it with the `!lk-start` command (see below)
- Disable notifications by default on the channels where the game happens (from *Notifications Settings*, in Discord server menu)

![Notification Settings menu preview](./notifications-settings-menu.png)

## How to play?

You can try this game on [my demo Discord server](https://discord.gg/4nhqwqXP5c), or install it on your own server by following the instructions above. In order to call the cat, users must post a message that contain one of the following keywords (and don't forget the question mark!).

- *Meow?*
- *Minou ?*
- *Miaou ?*

***The first user that make the cat show up wins!***

... Have a nice time with your community ;)

## Features

- Calling cats
- Show GIF when a cat has been found
- Options: language, auto-restart and automatically remove *Meow?* messages if you prefer
- Specify game channel or category (avoiding to totally ruin your Discord server with *Meow?* messages everywhere)
- Highscores: show your community members highscores, the total number of cats found on your server and in the World!

## Commands

The game can be started/restarted and configured by using *commands*, which are Discord message that starts by `!`. This is for now the only way to setup the game on your server. You can use the !lk-config- commands in order to configure the game or change the language. Here is the list of available commands.

### Gameplay commands

#### `!lk-start <channel or category name (optional)>`

Starts or restarts the game in your server. You can pass the name of one of your server's category or channel in order to limit the scope of the game (and eventually avoid users to call the cat in other channels).

If the named channel is a category, the game will happen in one of this category's channels. If the named channel is a text channel, the game will only happen in that channel. In any other case, the game will happen in a random "public" (where @everyone can write messages) channel of your server.

*Examples: `!lk-start` | `!lk-start Lost Kittens`*

#### `!lk-isplaying`

Checks if a game is currently running on your server or not.

### Configuration commands

#### `!lk-config-autorestart <0 for no, 1 for yes>`

Defines if you want the game to restart when the cat is found, or if you want to restart the game manually (using the !start command). You can use for value 1 (for yes) or 0 (for no).

*Example: `!lk-config-autorestart 1`*

#### `!lk-config-erasemessages <0 for no, 1 for yes>`

Defines if you want the messages of users calling the cat to be automatically deleted by the bot, or if you want to let the messages in the channels. You can use for value 1 (for yes) or 0 (for no).

*Example: `!lk-config-erasemessage 0`*

#### `!lk-config-language <0 for no, 1 for yes>`

Defines the language of the game on your server. For now, the only available values are: ***EN** (for English)* and ***FR** (for French)*.

Example: `!lk-config-language en`

### Other commands

#### `!lk-help`

Displays all the available commands of the Lost Kittens bot.

#### `lk-highscores`

Displays the 5 members that have found the most cats. This command also displays the total number of cats found on your server and in the World!

*Examples: `lk-highscores`*

#### `!lk-feedback`

Allow you to report a bug, request features, ask me anything, or just send me good vibes. Just follow this command of your message! :)

*Examples: `!lk-feedback This game is great!` | `!lk-feedback You've just ruined my server!`*
