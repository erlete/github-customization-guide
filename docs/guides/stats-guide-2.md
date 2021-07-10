---
title: "5. GitHub Stats (II)"
author: "Paulo Sánchez"
date: 2021-02-07
---

# 5. GitHub Stats (II)

***

Jstrieb's GitHub Stats is made of, esentially, a couple of Python scripts and a GitHub Actions workflow. It sounds pretty simple (which does not mean it took a whole lot of work to get it done), and thankfully, for its users, it is.

## Installation

### 1. Personal Access Token

First of all, if you want to use this functionality, you must generate a Personal Access Token (PAT) for GitHub itself. PATs are, in some way, "passwords" to partially or totally log in to the platform, which come in handy if you are using an Application Programming Interface (API), which would require some authentication method. It would be, to say the least, unsafe to provide to the API with your own GitHub password, which has master access to your account. Instead, PATs are used, since their permissions range can be restricted.

Let us follow the steps to generate a PAT, open another GitHub window if you may:

* On the upper right corner of the screen, click on your profile icon.
* Go to "Settings".
* On the left side of the screen you will see "Profile", "Account"... Go down to "Developer Settings".
* Again, on the left, you will see "Personal access tokens", click it.
* Click on "Generate new token" and follow the steps below:

If you followed the steps above, you will see a "Note" text box, in which you can add some insightful note about the usage of this PAT that you are going to create such as `github-stats` or any other name you like. You can choose freely. Below that, you will see a sizable amount of checkboxes with weird names (these are permission scopes), si do not get scared. Just check the `repo` one (note that it will also check all its children, which is totally fine) and then go down to the `user` one and check only the `read:user` one. Both of these are used for reading repositories' data and user data.

***

### 2. Repository Secrets

Again, let us follow some steps to get to the repository secrets page:

* Go to the repository where you want to install GitHub Stats.
* There is a navigation bar on top of the repository files redirecting to "Code", "Issues"... On the right, click on "Settings".
* On the left side of the screen you will see "Options", "Manage access"... Go down to "Secrets".
* Once you are in the "Secrets" screen, click on "New repository secret" and follow the steps below:

Now, you **must** name your secret exactly as `ACCESS_TOKEN` or else GitHub Stats will not work. In the "Value" text box, paste the PAT you obtained earlier.

***

Previous: [4. GitHub Actions](https://erlete.github.io/github-customization-guide/guides/actions-guide.html) | Next: [6. GitHub Pages](https://erlete.github.io/github-customization-guide/guides/pages-guide.html)
