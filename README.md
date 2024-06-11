# ft_irc

The goal of this project was to create a simple IRC server in C++.

## Usage

Build the project, by executing the Makefile in the root folder with :

```
make
```

Run the executable :

```
./ircserv [port] [password]
```

You can then connect to the server using any IRC client, we took Irssi as a reference :

```
irssi -c localhost -p [port] --password=[password]
```

You can use the following commands:
- `NICK` - Change nickname
- `QUIT` - Quit the server
- `JOIN` - Join a channel
- `PART` - Leave a channel
- `PRIVMSG` - Send a message
- `TOPIC` - Set or check a channel topic
- `MODE` - Set or check a user or channel mode
  - `i` : Set or remove the invite-only mode of a channel
  - `t` : Set or remove the restrictions of the TOPIC command to channel
operators
  - `k` : Set or remove the channel key (password)
  - `o` : Give or take channel operator privilege
  - `l` : Set or remove the user limit to channel
- `KICK` - Kick a user from a channel
- `INVITE` - Invite a user to a channel
