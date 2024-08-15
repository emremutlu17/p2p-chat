# P2P CHAT APPLICATION

Foobar is a Python library for dealing with word pluralization.

## Introduction

This Python project is a simple peer-to-peer chat application with functionality for viewing online users, initiating secure or unsecure chats, and viewing chat history. It utilizes threading for handling concurrent tasks, JSON for data interchange, and pyDes for message encryption and decryption.

## Features

- Welcome Animation: Displays a welcome ASCII art with a delay between lines.
- Menu System: Provides a CLI menu for navigating the application.
- Service Announcement: Broadcasts the user's presence on the network.
- Peer Discovery: Detects other users on the same network.
- Chat Functionality: Supports initiating and responding to chats, both secure and unsecure.

## Requirements
- Python 3.x
- pyDes library for encryption and decryption

```bash
pip install pyDes
python P2P_chat_app.py
```

Detailed Steps
1. Welcome Animation: The application starts with a welcome ASCII art animation.
2. Username Input: Enter your username when prompted.
3. Service Announcement and Peer Discovery: The application will broadcast your presence and listen for other users.
4. Chat Initiation:
Select the option to initiate a chat.
Choose secure (encrypted) or unsecure (plain text) chat.
5. Chat Responder: Listens for incoming chat messages and handles them appropriately.
6. View Chat History: Displays previous chat messages from message_log.txt.

## File Descriptions

- main.py: The main script containing all the functionality for the chat application.
- message_log.txt: A log file where all chat messages are stored (created upon first message).

## Security
- Encryption: Uses the pyDes library for DES encryption.
- Secure Chat: Encrypts messages before sending and decrypts them upon receiving.