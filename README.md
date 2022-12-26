try to use this https://github.com/interactions-py/interactions.py
for discord command dispatch

try to use python3.7 (3.7.9) from my dev nb
 - want to deploy to my raspberry pi which using python3.7.2
 - the same as python3.6, always install discord.py 0.16.x

try to use python3.10...
 - install the latest version of discord-py-interactions without discord.py dependency


#settings in discord#

discord developer [site](https://discord.com/developers/applications/)

fill-out app information and setup auth (can in-app auth)
 - bot, application.command
 - send message, embed links, add reactions
 - create auth url(using same permission)
 - go to link to auth for discord client app invite this bot
[optional] get client secret from the same page(can only renew for display)
 - if want to use programmable way to install bot automatically(perhaps? probably?)

[optional] get discord guild id(id for identify servers, channels or hashtags)
 - from discord client app, user settings-> advanced-> enable developer
 - right click from any of servers, channels or hashtags, get id from menu
 - leave guild id unset let bot interaction where invited in(seems that)
refer to https://interactionspy.readthedocs.io/en/latest/quickstart.html


#params for discord-py-interactions#

get bot token from developer site bot page(can only renew for display)
export to env `DISCORD_BOT_TOKEN`
- [option] export guild id to `DEFAULT_GUILD_ID` or just leave unset
coding.. just following discord-py-interactions [quickstart](https://interactionspy.readthedocs.io/en/latest/quickstart.html)


#openai api#

get openai api key from account page
export to env `OPENAI_API_KEY`
coding.. just following open ai [quickstart](https://beta.openai.com/docs/quickstart)
or just ask the chatgpt...
NOTE: completion response is a object contains choices listing results within text, use resp.choices[0].text
