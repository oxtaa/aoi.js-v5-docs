---
description: Setting a Hyperlink in an embed's description.
---

# Hyperlink

### Usage

```javascript
[Text Field](link 'Hover Field')
```

> `link` refers to an actual website link

> `Hover Field` can be anything you want

### Usage Example

```javascript
[aoi.js website](https://aoi.js.org 'aoi.js link')
```

{% hint style="danger" %}
Hyperlinks only work inside $description and embed fields.
{% endhint %}

### Example

{% tabs %}
{% tab title="index.js" %}
```javascript
client.command({
name: "hyperlink", 
code: `
$description[[Package](https://www.npmjs.com/package/aoi.js 'click')]` 
})
```
{% endtab %}
{% endtabs %}
