---
title: "3. GitHub Stats (I)"
author: "Paulo Sánchez"
date: 2021-02-07
---

# 3. GitHub Stats (I)

## [GitHub Stats Cards](https://github.com/anuraghazra/github-readme-stats/README.md#github-stats-card/)

A simple card able to display:

* Amount of stars of your repositories.
* Total commits, PRs and issues of your GitHub profile.
* Contributions to other projects / repositories.
* A GitHub profile rank, based on your activity and areas of interaction.

![Erlete's GitHub stats](https://github-readme-stats.vercel.app/api?username=erlete)

The stats card above can be displayed in your own README.md files using the [syntax for embedding images in markdown](https://erlete.github.io/github-customization-guide/guides/markdown-guide.html#image-links):

`![<placeholder text>](https://github-readme-stats.vercel.app/api?username=<your GitHub name>)`

Where `<placeholder text>` can be any text you want and `<your GitHub name>` must be, indeed, your GitHub name. The syntax for the card above looks like this:

`![Erlete's GitHub stats](https://github-readme-stats.vercel.app/api?username=erlete)`

The structure of the above graph consists in a link referring to a server-hosted platform that fetches your GitHub stats and displays them: `https://github-readme-stats.vercel.app/api?`.

This, however, is not related to your user in any way, so a `?username` parameter is required. Passed parameters follow a specific structure: `<parameter>=<value>`.

Therefore, the link referring to your GitHub statistics should look like this:

`https://github-readme-stats.vercel.app/api?username=<your username>`

In my case,

`https://github-readme-stats.vercel.app/api?username=erlete`

And that's it! Implementing this simple link in your README.md should display your stats correctly.

_Note: if you are unable to do so, that is because you have not checked this README.md source, so do it._

However, if you feel like something is missing here, I have got good news for you: [anuraghazra](https://github.com/anuraghazra/) though that too and decided to implement a wide range of customisation parameters.

In order to customise the graph, more parameters must be passed into the link. They follow a different structure than the `username` one, though: `&parameter=value`.

This example contains some parameters (which are explained in the list below). Take a look at it and get familiar with the structure:

`https://github-readme-stats.vercel.app/api?username=erlete&hide=stars,issues,prs,contribs,&hide_title=true&border_radius=40`

You might be wondering how that looks, so here is the result:

![](https://github-readme-stats.vercel.app/api?username=erlete&hide=stars,issues,prs,contribs,&hide_title=true&border_radius=40)

### Parameters

***
***

* Previous: [2. GitHub-flavored Markdown](https://erlete.github.io/github-customization-guide/guides/markdown-guide.html)
* Next: [4. GitHub Actions](https://erlete.github.io/github-customization-guide/guides/actions-guide.html)
