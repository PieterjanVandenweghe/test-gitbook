---
authorinformation:
  - null
  - Pieterjan Vandenweghe
keyword: null
---

# LF will be replaced by CRLF

## Condition

You get the error message `warning: LF will be replaced by CRLF` in a certain file when you want push the files to the cloud.

![](../../../.gitbook/assets/git-lf-replaced-crlf.png)

## Cause

These messages are due to incorrect default value of `core.autocrlf` on Windows. The concept of `autocrlf` is to handle the line endings transparently.

## Remedy

1. Open the local folder of your GitHub repository in Windows Explorer.
2. Open the config file in .git subfolder with a text editor like NotePad++.
3. Add the code `autocrlf = false` in the `[core]` section.

   ![](../../../.gitbook/assets/git-lf-replaced-crlf-remedy.png)

4. Save the file.

