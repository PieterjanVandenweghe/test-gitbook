---
authorinformation: null
---

# Cannot add untracked files

## Condition

If you are trying to[add untracked files](../ta_tracking_untracked_files.md), the following error might occur:

![](../../../../.gitbook/assets/warning_cr_lrf.png)

## Cause

In Unix systems the end of a line is represented with a line feed \(LF\). In Windows, a line is represented with a carriage return \(CR\) and a line feed \(LF\), thus \(CRLF\). When you get code from Git that was uploaded from a Unix system, they will only have an LF. If you are a single developer working on a Windows machine, and you don't care that Git automatically replaces LFs to CRLFs, you can turn this warning off. More information on this issue is available in [Git documentation](http://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration#Formatting-and-Whitespace).

## Remedy

1. Type `git config --global core.autocrlf false`.
2. Press Enter.

