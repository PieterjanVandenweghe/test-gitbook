---
authorinformation:
  - null
  - null
category: null
keyword: null
---

# Adjust the Preface of the WKFS document

1. Open the Preface ditamap of the document you’re working on in the **DITA Maps Manager**.

   ![](../../../../../.gitbook/assets/adjusting_wkfs_preface_1.png)

2. Right-click on the **Introduction** concept topic and select **Insert Before** &gt; **New…**.
3. Choose the **topic\_wkfs** file template, title it Preface and make sure to add the suffix of the type of document you’re working on to the file name.

   to\_preface\_ug.dita when you are working on the user guide

   ![](../../../../../.gitbook/assets/adjusting_wkfs_preface_2.png)

4. Select **Create**.
5. Select all child topics of the **Introduction** concept topic and drag them under the **Preface** title topic.

   ![](../../../../../.gitbook/assets/adjusting_wkfs_preface_4.png)

6. Delete the empty **Introduction** concept topic by right-clicking it and selecting **Remove from Disk**.
7. When the message Are you sure you want to move the selected topic\(s\) to the Recycle Bin? appears, select **Yes**.
8. Change the title of the **About this document** concept topic to a title more specific to the document you are working on.

   “About the SGMAS Workflow and User Guide”

9. Select all the other topics below this “About” concept topic, right-click and select **Organize** &gt; **Demote**.

   ![](../../../../../.gitbook/assets/adjusting_wkfs_preface_6.png)

10. Right-click the **Audience** concept topic and select **Edit Properties…**.
11. In the Edit Topic Reference Properties window, go to the **Attributes** tab and change the `@chunk` attribute to **to-content**.

    ![](../../../../../.gitbook/assets/adjusting_wkfs_preface_7.png)

    **Note:**

    You can use the **to-content** value on a parent topic, if you want its child topics to be displayed on the same \(html\) web page. This attribute-value pair has no effect on printed output.

12. Select **OK**.

