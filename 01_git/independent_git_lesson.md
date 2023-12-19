# Git Lesson

Git is another critical tool in a programmer's tool belt. It allows users to
easily save their work (commit) and look back (revert) if they every make a
mistake. It also allows users to easily experiment (branch) with new code so
they don't interfere with or break existing functionality. Finally, it provides
a means by which programmers can collaborate, allowing projects to move quickly
and integrate the skills of all.

This lesson involves several rounds of research, reflection, and application.

## Research Part 1:

Complete the Microsoft Learn "intro to git" course. The course is available at
https://learn.microsoft.com/en-us/training/modules/intro-to-git/ . You _will_
need to create a Microsoft account to access the tutorial (should be free),
but you _should not_ need to create an Azure sandbox. Instead, you can do all
of the commands on your own personal laptop. Whenever you see the phrase "Cloud
Shell", simply use your local version of shell.

> Make sure to watch the `Introduction to Git Recap` video.

## Reflection Part 1:

1. If you run the command `mkdir example && cd example && git init`, what have you done?
   ```


   ```
2. The most common git commands are `status`, `add`, and `commit` (usually in that order). Why?
   ```



   ```
3. Git is often described as "a chain of diffs". Why?
   ```



   ```
4. What is the difference a tracked file and an untracked file in git?
   ```



   ```

## Research Part 2:

Now, it's time to put your skills into action in a more complex way. Complete
https://learn.microsoft.com/en-us/training/modules/create-git-project/ . At the
end, you should have a simple git repository with a few commits in it.

## Reflection Part 2:

1. A lot of information about individual commits is shown when you run `git log`.
   In the space below, create an example `git log` entry and explain what each
   line means.
   ```




   ```
2. What does the `.gitignore` file do?
   ```
   


   ```
3. What does the `.git` folder do?
   ```
   


   ```
4. What command is equivalent to `cp FILE1 FILE2 && git rm FILE1 && git add FILE2`?
   ```
   


   ```
5. What is the difference between `rm FILE` and `git rm FILE`?
   ```
   
   

   ```

## Application:

### TIL Repository

To demonstrate your understanding of git, you are now going to move your TIL
entries from your TIL Google Doc to a git repository. To do this, you will create
a repository on UCLS's GitLab server and then `git push` your content up.

To accomplish this, complete the following steps:

1. Log into `https://gitlab.ucls.uchicago.edu` using your Google credentials
2. Create a `New project` (aka repository) called "Today I Learned"
   - The project should be **blank**
   - Make the project "slug" be `til`
   - Make sure the project is `Private`
3. Use `git clone` to pull down the newly created repository
   - Read the `README.md` file carefully, it has a **lot of useful information**
4. Create one file for every entry in your TIL Google Doc and copy in the content
   - Make sure to name the files something that is easy to understand
   - The resulting folder structure should be something like:
   ```
   - TIL Repository
      - README.md
      - shell
         - SHELL_ENTRY_FROM_TIL_GOOGLE_DOC_1.md (you can choose your own file name)
         - SHELL_ENTRY_FROM_TIL_GOOGLE_DOC_2.md (you can choose your own file name)
         - ...
      - git
         - GIT_ENTRY_FROM_TIL_GOOGLE_DOC_1.md (you can choose your own file name)
         - GIT_ENTRY_FROM_TIL_GOOGLE_DOC_2.md (you can choose your own file name)
         - ...
   ```
6. Give me (erizzi) access to your repository

### Git Back

The two lessons that you've completed so far (plus some future ones) are stored
in a repository on GitLab. This allows you to "collaborate". Therefore, I would
like you to clone the repository (gitlab.ucls.uchicago.edu/erizzi/intro-cs-extension)
and make at least one change to either this lesson or the shell lesson with a
new or improved question or some new content. Once you are done, push your changes.
