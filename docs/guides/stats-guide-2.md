---
title: "5. GitHub Stats (II)"
author: "Paulo Sánchez"
date: 2021-02-07
---

# 5. GitHub Stats (II)

***

Jstrieb's GitHub Stats are out made of, esentially, a couple of Python scripts and a GitHub Actions workflow. Thankfully, the developer put in the effort to make them very user-friendly.

This statistics card is able to display:

* The amount of stars of your repositories.
* Total amount of forks of your repositories.
* Contributions to other projects / repositories.
* Amount of changed code lines.
* Repository views.
* Repositories with contributions.

![](https://github.com/erlete/github-customization-guide/blob/master/github_stats/generated/overview.svg)

***

## Installation

***

### Personal Access Token

First of all, if you want to use this functionality, you must generate a Personal Access Token (PAT) for GitHub itself. PATs are, in some way, "passwords" to partially or totally log in to the platform, which come in handy if you are using an Application Programming Interface (API), which we are doing here, that would require some authentication method. It would be, to say the least, unsafe to provide to the API with your own GitHub password, which has master access to your account. Instead, PATs are used, since their permissions' range can be restricted.

#### PAT Generation Steps

* On the upper right corner of the screen, click on your profile icon.
* Go to ***Settings***.
* On the left side of the screen you will see *Profile*, *Account*... Go down to ***Developer Settings***.
* Again, on the left, you will see three options. Go to***Personal access tokens***.
* Click on ***Generate new token*** and follow the steps below:

If you properly followed the steps above, you will see a ***Note*** text box, in which you can add some insightful note about the usage of this PAT, such as `github-stats` or any other name you like. **You can choose freely**. Below that, you will see a sizable amount of checkboxes with weird names, the permission scopes. Just check the `repo` one (note that it will also check all its children, which is totally fine) and then go down to the `user` one and check only the `read:user` one. These permissions are used for reading repositories' data and user data, respectively.

Remember the generated PAT, which should be a weird collection of alphanumeric and even symbolic values. Note that, if you forget it, you will not be able to take another look at it unless you regenerate it, which will delete the previous PAT and produce a new one.

***

### Repository Secrets




#### Secret Generation Steps

* Go to the repository where you want to install GitHub Stats.
* There is a navigation bar on top of the repository files with links to *Code*, *Issues*... On the right, click on ***Settings***.
* On the left side of the screen you will see *Options*, *Manage access*... Go down to ***Secrets***.
* Click on ***New repository secret*** and follow the steps below:

Now, **you must name your secret exactly as** `ACCESS_TOKEN` or else GitHub Stats will not work. In the ***Value*** text box, paste the PAT you obtained earlier.

***

Previous: [4. GitHub Actions](https://erlete.github.io/github-customization-guide/guides/actions-guide.html) | Next: [6. GitHub Pages](https://erlete.github.io/github-customization-guide/guides/pages-guide.html)
