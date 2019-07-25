# A Petclinic import demo from Jenkins X

This repo is created just by importing my [Petclinic repo with Kaniko](https://github.com/dcanadillas/petclinic-kaniko) with Jenkins X.

- Clone original repo from the terminal with git clone https://github.com/dcanadillas/petclinic-kaniko petclinic-jx.
- Remove git references rm -rf petclinic-jx/.git* (this is just for importing directly from local and create a new repo automatically)
- Now, create Jenkins X project by importing from the local repo into a new GitHub repository:

```
  jx import --git-username <git_username> --org <git_org> --name petclinic-jx -m YAML
```
