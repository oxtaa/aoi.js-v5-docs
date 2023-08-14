---
description: Here you can see how to setup variables.
---

# Variables

> It must be inside of your main file, in most of the cases this is `index.js`

### Usage

```javascript
client.variables({
variable: "value"
})
```

#### Example

```javascript
client.variables({
money: 0
})
```

#### Multiple Variables

```javascript
client.variables({
money: 0,
oxta: "developer"
})
```

> Integers do not need a string

### Channel Variables

> The variable value will be saved to a channel

#### Setting the channel variable

```php
$setChannelVar[variable;value;channelID (optional)]
```

#### Retrieving the channel value

```php
$getChannelVar[variable;channelID (optional)]
```

### Message Variables

> The variable value will be saved to a message

#### Setting the message variable

```php
$setMessageVar[variable;value;messageID]
```

#### Retrieving the message variable value

```php
$getMessageVar[variable;messageID]
```

### Global Variables

> The value will be assigned to everyone and it will be the same for every guild

#### Setting the global variable

```php
$setVar[Variable;Value]
```

#### Retrieving the global variable value

```php
$getVar[Variable]
```

### Global User Variables

> The value will be assigned to a user and it will be the same for every guild

#### Setting the global user variable

```php
$setGlobalUserVar[Variable;Value;User ID (optional)]
```

#### Retrieving the global user variable value

```php
$getGlobalUserVar[Variable;User ID (Optional)]
```

### Local User Variables

> The value will be assigned to a user and it will be assigned per guild

#### Setting the local user variable

```php
$setUserVar[Variable;Value;User ID (Optional);Guild ID (Optional)]
```

#### Retrieving the local user variable value

```php
$getUserVar[Variable;User ID (Optional);Guild ID (Optional)]
```

### Server Variables

> The value will be assigned per Guild.

#### Setting the server variable

```php
$setServerVar[Variable;Value;Guild ID (Optional)]
```

#### Retrieving the server variable value

```php
$getServerVar[Variable;Guild ID (Optional)]
```
