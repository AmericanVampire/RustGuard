<p align="center">
<img src="https://i.imgur.com/OlaSRS2.png" width="500">
</p>

<h1 align="center"><em><b>RustGuard</b></em></h1>

RustGuard is a self-hosted NodeJS Discord bot that integrates with the Rust+ Companion system to provide automation, monitoring, and team coordination tools for Rust servers.

RustGuard allows players to monitor their base, receive alerts, control smart devices, and communicate with teammates directly through Discord.

---

## Features

• Receive notifications for in-game events such as Patrol Helicopter, Cargo Ship, Chinook 47, and Oil Rig activation.  
• Control Smart Switches or groups of switches directly from Discord or in-game team chat.  
• Configure Smart Alarm alerts that notify Discord or team chat when triggered.  
• Monitor storage containers or tool cupboard upkeep using Storage Monitors.  
• View live server information including events and team member status.  
• Send messages between Discord and in-game team chat.  
• Track player activity on the server using integrated monitoring tools.  
• Access multiple quality-of-life commands from Discord or in-game chat.

---

## Documentation

Documentation for RustGuard explains how to configure, deploy, and operate the bot.

Refer to the docs folder for setup instructions and feature explanations.

---

## Credentials

RustGuard requires authentication credentials in order to connect to the Rust+ Companion system.

Generate the required credentials before starting the bot and place them in the credentials directory.

---

## Running RustGuard

Open a terminal in the project directory and run:

npm start

This will start the RustGuard bot instance.

---

## Updating RustGuard

Depending on your operating system you can run:

update.bat

or

./update.sh

This will update the project files and dependencies.

---

## Running RustGuard with Docker

docker run --rm -it \
-v ${pwd}/credentials:/app/credentials \
-v ${pwd}/instances:/app/instances \
-v ${pwd}/logs:/app/logs \
-e DISCORD_CLIENT_ID=YOUR_CLIENT_ID \
-e DISCORD_TOKEN=YOUR_TOKEN \
--name rustguard rustguard

or

docker-compose up -d

Ensure the correct values are set for DISCORD_CLIENT_ID and DISCORD_TOKEN.

---

## RustGuard Overview

RustGuard is designed to be a customizable self-hosted automation system for Rust servers. It provides Discord integration, smart device control, event notifications, and team coordination tools to enhance gameplay and base monitoring.

Because RustGuard is self-hosted, it can be customized, extended, and adapted to suit individual server needs.
