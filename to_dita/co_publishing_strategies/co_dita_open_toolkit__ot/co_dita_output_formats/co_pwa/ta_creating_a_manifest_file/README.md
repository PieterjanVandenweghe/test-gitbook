---
authorinformation:
  - null
  - Pieterjan Vandenweghe
keyword: null
---

# Creating a manifest file

The manifest file tells your browser about the progressive web app and how it should be installed when used on user's desktop or webapp. A manifest file includes:

* The app name.
* The icons the app should use.
* The URL that should be opened when the app is launched.

The manifest file is added to the root folder of your website.

```text
{
"name":"Flow PWA demo",
"short_name":"PWA",
"start_url":"/index.html",
"scope":"./",
"icons":[
{"src":"/android-chrome-192x192.png","sizes":"192x192","type":"image/png"},
{"src":"/android-chrome-512x512.png","sizes":"512x512","type":"image/png"},
{"src":"/apple-touch-icon.png","sizes":"180x180","type":"image/png"},
{"src":"/favicon-16x16.png","sizes":"16x16","type":"image/png"},
{"src":"/favicon-32x32.png","sizes":"32x32","type":"image/png"}
],
"theme-color":"#f00",
"background_color":"#f00",
"display":"standalone"
}
```

