---
authorinformation:
  - null
  - Pieterjan Vandenweghe
  - Yves.Barbion
keyword: null
---

# GitHub essentials and workflow

After installing the necessary tools and creating an account, it's time to get familiar with the essential definitions from GitHub and the default workflow.

* **Repository**

  A repository is used to organize single projects. It can contain several folders and files. At Flow bv we will create one repository per customer.

* **Template repository**

  A repository that is used as a template for other repositories. Whenever you create a new repository, you have the option to clone the structure from an existing template repository.

* **Branch**

  A branch is the way to work on different version of your project. By default a repository has a branch named `master`. You can create extra branches depending on the projects you are working on.

* **Master branch**

  The master branch is the default branch in a repository. This branch is considered the final version and is not intended to be used as a working copy. The idea is to create and work on a local branch and when the local branch is approved, you can store the final version on the `master` branch.

* **Push**

  This is the mechanism to synchronize your local changes to the cloud.

* **Pull origin**

  This is the mechanism to download latest changes from the cloud to your local copy.

* **Pull request**

  This is the mechanism to merge the changes from a local branch to another branch or the `master` branch. Once you created a pull request, this has to be confirmed by an administrator before it's final.

* **Merge**

  This is the mechanism where the changes from one or more collaborators are merged into one single version.

* **Conflicts**

  This is the mechanism where the changes from one or more collaborators prevent GitHub to merge the files. In the case of a conflict you need to resolve each conflict before you can synchronize the files to the cloud or create a pull request.

* **Fork**

  This is the mechanism to download a local copy of someone else's repository. It's a kind of bridge between your personal copy and the original repository.

* **.gitignore**

  A file in which you can save file names or file extensions to be ignored when pushing local files to the cloud.

* **.gitkeep**

  An empty file you can use to store in empty folders if you want to keep the folder structure. Folder structures without files are by default ignored by GitHub. This file is typically used in a template repository where you want to create a default folder structure for your projects.

This is how a typical GitHub workflow looks like at Flow bv:

![](../../../../.gitbook/assets/git-workflow.png)

* **1**

  Master branch

* **2**

  Writing branch

* **3**

  Local copy on your desktop from the writing branch.

* **4**

  Fetch or pull the files from the writing branch in the cloud and copy it into your local copy.

* **5**

  Push the files from your local copy to the writing branch in the cloud.

* **6**

  Request \(Pull request\) to merge the files from the writing branch to the master branch.

* **7**

  Optional extra review cycle.

* **8**

  Merge the writing branch again with the master branch to deploy the final version of the product.

