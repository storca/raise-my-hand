# raise-my-hand
A Discord bot made to inform people that you raise your hand by renaming users

## Description
The bot renames the people who react to his mesage so that they are brought up in the voice channel. When people stop *virtually* raising their hand, the bot renames them to their previous nickname. Moreover, the bot cleans request messages and his messages itself so the tchat doesn't get spammed.

This bot is made for a single-server use.

## Usage
### Start a "raise your hand" event

    {cmd_prefix}q

*The bot sends a message in the current context (eg: #channel) and adds a reaction to it. All the people that add a reaction are renamed with the prefix, people who remove their reaction are renamed with the pseudo they used when they added the reaction*

### Stop the "raise your hand" event

    {cmd_prefix}e

*Renames all people who "raised their hand" back to their default nicknames, deletes it's "Raise your hand!" message and the request message*

## Start the bot
### Install it
    git clone https://github.com/storca/raise-my-hand.git
    cd raise-my-hand

Change the settings of the bot in rmh_constants.py *(all settings are detailled in the file)*

Then run the bot

    pip3 install -r requirements.txt