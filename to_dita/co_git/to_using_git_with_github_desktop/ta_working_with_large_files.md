---
authorinformation:
  - null
  - Yves
---

# Working with large files: Git Large File Storage

To keep GitHub fast for everyone, GitHub does not allow files larger than 100 MB to be tracked in repositories. This also means that you cannot push files larger than 100 MB to the Git repo. You will get an error message when you try to do so.

But... luckily there is and open-source Git extension for versioning large files: [Git Large File Storage \(LFS\)](https://git-lfs.github.com/)

1. Close your GitHub client.
2. Download and install git-lfs here: [https://git-lfs.github.com/](https://git-lfs.github.com/).
3. Once downloaded and installed, set up Git LFS for your user account by running in the DOS command line:

   ```text
   git lfs install
   ```

   **Note:** You only need to run this once per user account.

4. In DOS, go to your GitHub repository.

   `c:\cd e:\_github\customer_name`

5. Select the file types you'd like Git LFS to manage \(or directly edit your .gitattributes\).

   ```text
   git lfs track "*.zip"
   ```

   **Note:** You can configure additional file extensions at anytime.

6. Make sure .gitattributes is tracked.

   ```text
   git add .gitattributes
   ```

   **Note:**

   Defining the file types Git LFS should track will not, by itself, convert any pre-existing files to Git LFS, such as files on other branches or in your prior commit history. To do that, use the [git lfs migrate\[1\]](https://github.com/git-lfs/git-lfs/blob/master/docs/man/git-lfs-migrate.1.ronn?utm_source=gitlfs_site&utm_medium=doc_man_migrate_link&utm_campaign=gitlfs) command, which has a range of options designed to suit various potential use cases.

7. Start your GitHub client again and commit and push like a beast!

