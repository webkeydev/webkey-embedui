# Webkey EmbedUI

## Overview
This is a Javascript library. With this tool you can integrate the Webkey real time interface (Webkit) into your HTML page.

## Usage
Load the **wkembed.js** file into your HTML page and define a **div** container with unique id for the integration.
You must set three parameters for the library initialization:
1. device reference: With this parameter you can refer to your device. This parameter  could be **publicid**, **serial** or **devicenick**. You can found this these values on the [Dashboard interface](https://webkey.cc/dashboard).
2. remote-admin token: See the [Dashboard API documentation](https://https://webkey.cc/apidoc#devices-request-new-remote-admin-token-get) for more detailes. 
3. container id: ID of your DIV container where you would like to load the Webkit.
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

## Example
In the index.html you can see the example.
