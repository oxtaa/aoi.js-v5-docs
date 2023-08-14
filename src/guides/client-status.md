---
description: How to setup a Bot Status
---

# Client Status

#### Setting a Client Status:

You need to enter the following, in your main index.

#### Usage:

```javascript
client.status({
  text: "TEXT",
  type: "PLAYING",
  time: 12
})
```

#### Adding multiple Client Status:

```javascript
client.status({
  text: "TEXT1",
  type: "PLAYING",
  time: 12
})

client.status({
  text: "TEXT2",
  type: "WATCHING",
  time: 12
})
```

#### Different Types:

* PLAYING
* WATCHING
* LISTENING
* STREAMING
* COMPETING

#### Client Status Method:

If you want to change the Client Discord Status use the following:

```diff
+ status: "type"
```

```javascript
client.status({
  text: "TEXT",
  type: "PLAYING",
  status: "idle",
  time: 12
})
```

#### Different Status Types:

* `idle`
* `dnd`
* `online`
* `invisible`

#### Streaming URL Method:

Streaming-Status supports `YouTube-Video-URLs` or `Twitch-Stream-URLs`.

If you want to enter an URL, Enter the following

```diff
+ url: "URL"
```

```javascript
client.status({
text: "TEXT", 
type: "STREAMING", 
url: "URL"
})
```

> Make sure your `type` is `STREAMING`

#### Mobile Status

```diff
+ mobilePlatform: true
```

```javascript
const oxi = require("oxi.js")

const client = new oxi.Client({
  token: "Discord bot Token",
  prefix: "Your Prefix",
  intents: ["GUILDS", "GUILD_MESSAGES"],
  mobilePlatform: true
})
```

![Example](../discord-examples/assets/image%20\(62\).png)
