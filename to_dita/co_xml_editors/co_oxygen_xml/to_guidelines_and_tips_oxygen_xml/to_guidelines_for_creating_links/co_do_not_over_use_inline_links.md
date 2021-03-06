---
authorinformation:
  - null
  - Kimberley.De.Moor
category: User Guide
keyword: null
---

# Do not overuse inline links

It is easy to overuse inline links in your text, making it confusing to the reader. It is important to use them only when necessary and keep in mind the following guidelines:

## Avoid inline links to tables and figures in a topic

Keep your topics short and self-contained. These links can become difficult to maintain when you update your topics, for instance by deleting a table or moving it to a different topic. They can also make it difficult to re-use topics. Instead, you can consider re-using the table or the figure somewhere else in the form of a content reference \([conref](../../../../to_different_levels_of_content_re_use/co_using_conrefs.md)\).

## Create inline links to repeated steps

You might use phrases such as ‘Repeat step 2 to add each topic to the DITA map’. In this case you will need to update this phrase every time you add a step before ‘step 2’. You can solve this by adding an `xref` element that links to the relevant step. In doing so, every time the numbering changes in the steps, the `xref` element will ensure the text changes automatically.

## Create inline links to high-level tasks

If you have a manual that contains a task flow with too many task topics, the user might start to lose track of the big picture. As these tasks might be spread throughout your DITA map, you might not be able to take advantage of the default linking system. In this case, you can use inline links to show users a roadmap of the task flow they will have to follow. This way, they can plan for tasks they will need to complete in the future.

