---
authorinformation:
  - null
  - Pieterjan Vandenweghe
keyword: null
---

# Declaring the DOCTYPE in the topic templates

When you create a DITA-OT specialization, you need to make sure you can see the correct elements and attributes when you start to write. You can do this by adjusting the DOCTYPE in your DITA templates.

1. Open the default topic template.

   ```text
   <?xml version="1.0" encoding="UTF-8"?>
   <!DOCTYPE topic PUBLIC "-//OASIS//DTD DITA Topic//EN" "topic.dtd">
   <topic id="topic_ajq_zbw_2lb">
       <title></title>
       <body>
           <p></p>
       </body>
   </topic>
   ```

2. Replace the standard PUBLIC ID in the `!DOCTYPE` with the PUBLIC ID of your DITA-OT plug-in.

   This is the `@publicId` attribute you declared in the Catalog XML file. See [Declaring files in the DITA catalog file](declaring_files_in_the_dita_catalog.md).

   ```text
   <?xml version="1.0" encoding="UTF-8"?>
   **<!DOCTYPE topic PUBLIC "-//FLOW BVBA//DTD Agilent DITA specialization topic//EN" "topic.dtd"\>**
   <topic id="topic_ajq_zbw_2lb">
       <title></title>
       <body>
           <p></p>
       </body>
   </topic>
   ```

Your DITA-OT plug-in is ready for use. Add the plug-in to your DITA-OT plug-in folder and install it correctly as explained in [Installing an extra DITA-OT plug-in](../../co_publishing_strategies/co_dita_open_toolkit__ot/co_installing_an_extra_dita_ot_plugin/).

