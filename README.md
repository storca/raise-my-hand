# VHBot
A Discord bot made to inform people that you raise your hand by renaming users

## Description
The bot renames the people who react to his mesage so that they are brought up in the voice channel. When people stop *virtually* raising their hand, the bot renames them to their previous nickname. Moreover, the bot cleans request messages and his messages itself so the tchat doesn't get spammed.

This bot is made for a single-server use.

## Usage

### Tell the bot to join your channel if you want a sound

    {cmd_prefix}join

### Tell the bot to leave the channel

    {cmd_prefix}leave

### Start a "raise your hand" event

    {cmd_prefix}q

*The bot sends a message in the current context (eg: #channel) and adds a reaction to it. All the people that add a reaction are renamed with the prefix, people who remove their reaction are renamed with the pseudo they used when they added the reaction*

### Stop the "raise your hand" event

    {cmd_prefix}e

*Renames all people who "raised their hand" back to their default nicknames, deletes it's "Raise your hand!" message and the request message*

## Start the bot
### Install it
    git clone https://github.com/storca/vhbot.git
    pip3 install -r requirements.txt
    cd raise-my-hand
    cp default.conf instance.conf

Change the settings of the bot in instance.conf *(all settings are detailled in the file)*

Then run the bot

    python3 vhbot.py
