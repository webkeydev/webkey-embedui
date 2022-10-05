# Webkey EmbedUI

## Overview
This is a Javascript library. With this tool you can integrate the Webkey real time interface (Webkit) into your HTML page.

## Usage
Load the **wkembed.js** file into your HTML page and define a **div** container with unique id for the integration.

```html
<div id="wk-container"></div>
...

<script>
    app = new WKEmbedUI({
      publicid:'[DEVICE-ID]',
      raToken: '[REMOTE-ADMIN-TOKEN-UUID]',
      container: 'wk-container'
    });
</script>
```

### Parameters
#### Mandatory pamaters

1. device reference: With this parameter you can refer to your device. This parameter  could be **publicid**, **serial**. You can see this these values on the [Dashboard interface](https://dashboard.webkeyapp.com).
2. remote-admin token: See the [Dashboard API documentation](https://webkey.cc/apidoc#devices-request-new-remote-admin-token-get) for more detailes.
3. container id: ID of your DIV container where you would like to load the Webkit.

#### Optional pamaters
1. extlink=disabled: Disable the links to the Dashboard interface

## Example
In the *index.html* you can see the example.
