---
authorinformation: null
---

# Reusing software strings in your technical documentation

## Challenge

Suppose you have a software application accompanied with documentation, such as a user guide, online help or an API reference guide. You obviously want to the text in the documentation to be consistent with the text in the user interface \(dialog boxes, menu commands, display messages...\). And of course you want this in the translations too.

You may find this consistency in the first version of the documentation, but is this also the case in later versions as the software gets updated? Maybe not if the text from the user interface has been typed over in the documentation. Each update of the software may then mean you will have to scrutinize the complete documentation set to find and fix inconsistencies, in the \(English\) source language and in the translations.

## Solution

Fortunately, there is a better way to deal with this challenge: reusing the text from your software applications, aka the "software strings", with a dynamic link in your documentation. The process goes as follows:

![](../../.gitbook/assets/software_strings_process.svg)

1. You export the text from your software application to a structured file format, for example XML, CSV or JSON. Or maybe you already have that text in such a format available ?
2. We transform that file to a DITA file, where the software strings become reusable components.
3. The technical writers no longer **type** the software strings in their documentation, but they **drag** them from a repository of reusable components into their content, thus creating a dynamic link.
4. As the software gets updated, we only perform steps 1 and 2: export the text from the user interface again and retransform software strings file into a repository or warehouse of reusable components.
5. And, of course, step 4 works for updates of the translations too: export the text from the translated user interface again, transform it and you're done!

Isn't that nice?

## Interested?

Drop us an email: [info@flowtime.be](mailto://info@flowtime.be)

