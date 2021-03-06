---
authorinformation:
  - null
  - Kimberley.De.Moor
category: User Guide
keyword: null
---

# Add the glossary term to the glossary map

Your publication needs to contain a glossary map. If this is not the case yet, add a ditamap to your publication.

**Note:** You can give this ditamap any name you like, but for clarity’s sake, we suggest you call it \_Glossary.

1. Open the \_Glossary ditamap in the **DITA Maps Manager**.
2. Right-click the \_Glossary ditamap and select **Append child** &gt; **Glossary Reference…**.
3. Select your newly created glossentry topic.
4. Click **Insert and close**.

   Oxygen adds the topic to the \_Glossary ditamap as a `glossref` element but gives an error message that the `glossref` element needs a key.

5. Open the publication or the \_Glossary ditamap in the Author window.
6. Select the newly added `glossref` element.
7. Fill out its `@keys` attribute in the Attributes window.

   You can give this `@keys` attribute any name you like, but for clarity’s sake, we suggest you give it the same name as its `glossterm` or title.

8. Save your changes.

