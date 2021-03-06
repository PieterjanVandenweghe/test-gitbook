---
authorinformation: null
---

# Step 2: Conversion — Save the FrameMaker files as MIF \(Maker Interchange Format\)

If you clean up the source files in a FrameMaker version later than version 11, you need to save all the files as MIF once you're done with the cleanup. You need to do this because the conversion plugin MIF2Go only works with FrameMaker 11.

You can save the .fm files as .mif one by one but we also have a script \(SaveAllAsMifAndPdf2.jsx\) which saves all the files in a FrameMaker book as MIF in one go. Once you have saved your files as MIF, you also need to create a FrameMaker book file which holds the MIF files in the same order and the original FrameMaker book. You need to save that FrameMaker book as MIF too to be able to open it in FrameMaker 11.

1. Open the original FrameMaker book in a later version of FrameMaker, for example 2019 or 2020.
2. Save all the .fm files as .mif:
   * If you **don't** have the SaveAllAsMifAndPdf2.jsx script, open the files in the book and then choose **File** &gt; **Save as** and select **MIF 2019 \(\*.mif\)**.

     **Note:** Do not select **MIF 7.0** because this version of MIF does not support Unicode!

   * If you **do** have the SaveAllAsMifAndPdf2.jsx script installed, click somewhere in the book and choose **Edit** &gt; **Save All Components as MIF**.
3. Create a new FrameMaker book file and add all the MIF files to the book.
4. Save the book itself as MIF too: **File** &gt; **Save Book As** &gt; **MIF 2019 \(\*.mif\)**.

The next step is to [save the MIF files as DITA](conversion_save_the_mif_files_as_dita.md).

