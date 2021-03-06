---
authorinformation:
  - null
  - Pieterjan Vandenweghe
keyword: null
---

# Updating the head of the HTML page

In the procedure [Making the service worker ready to use](ta_making_the_service_worker_ready_to_use.md) you added a script to the `head` of the index.html. This script referenced to a file service-worker.js for testing purposing. After installing and configuring the Workbox configuration, the service-workers.js became a template file for the sw.js in which all files to be cached are stored. This means we also have to update our script in the index.html file.

1. Open the index.html page in a text editor.
2. Search for `navigator.serviceWorker.register('/service-worker.js');` and replace it with `navigator.serviceWorker.register('/sw.js');`.
3. Add the link to the manifest and in the `head`.

   ```text
   <head>
   ...**
   <link href="/manifest.json" rel="manifest" /\>**
   ...
   </head>
   ```

