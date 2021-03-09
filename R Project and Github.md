Pre-requisites
--------------
- Install R, R Studio, Git
- Create your account at GitHub

Setup Git on RStudio (is necessary only once)
---------------------------------------------
1. Inform Git your name, and email. Use the same email associated with your GitHub account.
  - On RStudio:
     ```
      usethis::use_git_config(user.name = "Gustavo Xavier", # Your name
                          user.email = "gcx@academico.ufpb.br") # Your e-mail
      ```
   - or on Git:
      ```
      $ git config --global user.name "Gustavo Xavier"

      $ git config --global user.email gcx@academico.ufpb.br
      ```

2. Create a new token on GitHub for your machine
      ```
      usethis::browse_github_token()
      ```
I suggest that you change the name of the token, to know which computer you are linking to.
3. Copy your token and paste on .Renviron file
  - To open .Renviron file run the command below:
      ```
      usethis::edit_r_environ()
      ```
  - Restart R Studio (CTRL + SHIFT + F10)

Create Repository from R Studio
-------------------------------
```
usethis::create_project("Folder/ProjectPath")
usethis::use_git()
usethis::use_github()

```

About .gitignore
----------------
- [GitIgnore topic of GitHub manual](https://githubtraining.github.io/training-manual/#/23_gitignore)
- [Collection of .gitignore templates based on popular programming languages](https://github.com/github/gitignore)
- [R Template](https://github.com/github/gitignore/blob/master/R.gitignore)


Others
------
- [usethis package documentation](https://usethis.r-lib.org/reference/create_package.html)
