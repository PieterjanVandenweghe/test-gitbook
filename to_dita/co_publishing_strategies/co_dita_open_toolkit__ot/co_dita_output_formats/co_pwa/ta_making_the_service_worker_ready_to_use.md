---
authorinformation:
  - null
  - Pieterjan Vandenweghe
keyword: null
---

# Making the service worker ready to use

This procedures assumes you have an existing webhelp or website and the website is online to test the scripts.

1. Open the root folder of your website.
2. Create a new file service-worker.js.
3. Open the file and add this code:

   ```text
   console.log('Hello from service-worker.js')
   ```

4. Open the index.html file in the root folder and add this code the `head`

   ```text
   <script>
   // Check that service workers are supported
   if ('serviceWorker' in navigator) {
     // Use the window load event to keep the page load performant
     window.onload = function() {
       navigator.serviceWorker.register('/service-worker.js');
     };
   }
   </script>
   ```

5. Go to the website in your default browser and open the **Developer tools** **\(CTRL+SHIFT+I\)**
6. Choose the **Console** tab and check if you see the following message Hello from service-worker.js

   ![](../../../../../.gitbook/assets/pwa-service-workers-hello-test.png)

   If you don't see the message, start the procedure again from the start.

7. Open the `service-worker.js` again and the following code to the file:

   ```text
   importScripts('https://storage.googleapis.com/workbox-cdn/releases/5.0.0/workbox-sw.js');

   if (workbox) {
     console.log(`Yay! Workbox is loaded 🎉`);
   } else {
     console.log(`Boo! Workbox didn't load 😬`);
   }
   ```

8. Open the **Console** tab again in the **Developer tools** of your default browser and check if you see the following message:

   ```text
   Hello from service-worker.js
   Yay! Workbox is loaded 🎉
   ```

   ![](../../../../../.gitbook/assets/pwa-service-workers-workboxloaded-test.png)

The service worker is ready to be used in a PWA environment.

**Note:**

When you use the [Workbox Quick start guide](https://developers.google.com/web/tools/workbox/guides/get-started) in parallel, you can skip the Importing Workbox section and go directly to [Precache Files with Workbox CLI](https://developers.google.com/web/tools/workbox/guides/precache-files/cli).

**Related information**

