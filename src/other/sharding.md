# Sharding

{% hint style="danger" %}
Sharding is only necessary for bots in 2,000+ Guilds
{% endhint %}

#### How to shard

```javascript
const client = new oxi.Client({
    sharding: true,
    shardAmount: 2,
    token: "token",
    prefix: "prefix"
})
```

#### Finding current guild's shard ID

```javascript
client.command({
    name: "shardID",
    code: `Guilds Shard: $shardID`
})
```

{% hint style="danger" %}
Sharding can lead to high ping/response time and depending your host, can use a lot of memory and disk space
{% endhint %}
