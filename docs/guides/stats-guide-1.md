---
title: "3. GitHub Stats (I)"
author: "Paulo Sánchez"
date: 2021-02-07
---

# 3. GitHub Stats (I)

***

## GitHub Stats Cards

A simple card able to display:

* The amount of stars of your repositories.
* Total commits, PRs and issues of your GitHub profile.
* Contributions to other projects / repositories.
* A GitHub profile rank, based on your activity and areas of interaction.

![Erlete's GitHub stats](https://github-readme-stats.vercel.app/api?username=erlete)

***

The structure of the above graph consists in a link referring to a server-hosted API that fetches your GitHub stats and displays them: `https://github-readme-stats.vercel.app/api`. The content of said link can be displayed in your own README.md files using the [syntax for embedding images in markdown](https://erlete.github.io/github-customization-guide/guides/markdown-guide.html#image-links):

`![<placeholder text>](https://github-readme-stats.vercel.app/api)`

Where `<placeholder text>` can be any text you want. Note, however, that this link is not, in any way related to your profile. This can be achieved by passing parameters into it. Parameters act as additional settings that allow customization of the stats' interface. They follow a specific structure:

`?<parameter name>=<value>`

Yet, if more than one parameter is passed, the structure is as follows:

`?<parameter 1 name>=<value>&<parameter 2 name>=<value>&...`

The first parameter required by the URL is the `username` one, which takes any GitHub profile name as value:

`https://github-readme-stats.vercel.app/api?username=<your username>`

My GitHub stats URL looks like this:

`https://github-readme-stats.vercel.app/api?username=erlete`

This is it! You have successfully set up your own GitHub stats display... but you might want to customize it, so take a look at the chapter below.

### Parameters

In this section there are two main indexes, ordered by [alphabetical order of the parameters](https://erlete.github.io/github-customization-guide/guides/stats-guide-1.html#alphabetical-order) and [parameters' area of application](https://erlete.github.io/github-customization-guide/guides/stats-guide-1.html#area-of-application). These indexes follow a specific structure:

* `Parameter identifier (name)`
	* Brief usage description
		* `Generic value structure`

#### Alphabetical Order

* `bg_color`
	* Sets card's background color or [gradient].
		* `hexadecimal color code`
* `border_color`
	* Sets border color.
		* `hexadecimal color code`
* `border_radius`
	* Sets border radius.
		* `positive value`
* `cache_seconds`
	* Sets the cache header manually.
		* `value from 1800 to 86400`
* `count_private`
	* If `true`, stats from private repositories are also gathered.
		* `true` `false`
* `custom_title`
	* Sets a custom title for the card.
* `disable_animations`
	* Disables animations for the card.
* `hide`
	* Takes one or many values and hides specific stats from the card.
		* `stars` `commits` `prs` `issues` `contribs`
* `hide_border`
	* If `true`, sets card's border as hidden.
		* `true` `false`
* `hide_rank`
	* If `true`, sets the rank as hidden.
		* `true` `false`
* `hide_title`
	* If `true`, sets card's title as hidden.
		* `true` `false`
* `icon_color`
	* Sets icon color.
		* `hex color code`
* `include_all_commits`
	* If `true`, all performed commits are counted.
		* `true` `false`
* `line_height`
	* Sets line height between text lines.
		* `positive value`
* `locale`
	* Sets card's language.
		* `cn` `de` `es` `en` (...)
* `show_icons`
	* If `true`, sets icons as hidden.
		* `true` `false`
* `text_color`
	* Sets text color.
		* `hex color code`
* `theme`
	* Sets a preset collection of parameters related to customization options.
		* [`one of the avaliable themes`](https://github.com/anuraghazra/github-readme-stats/blob/master/themes/README.md#stats)
* `title_color`
	* Sets title color.
		* `hex color code`

#### Area of application

##### Functionality

* `cache_seconds`
	* Sets the cache header manually.
		* `value from 1800 to 86400`
* `count_private`
	* If `true`, stats from private repositories are also gathered.
		* `true` `false`
* `hide`
	* Takes one or many values and hides specific stats from the card.
		* `stars` `commits` `prs` `issues` `contribs`
* `include_all_commits`
	* If `true`, all performed commits are counted.
		* `true` `false`
* `locale`
	* Sets card's language.
		* `cn` `de` `es` `en` (...)

##### Customization

* `bg_color`
	* Sets card's background color or [gradient].
		* `hexadecimal color code`
* `border_color`
	* Sets border color.
		* `hexadecimal color code`
* `border_radius`
	* Sets border radius.
		* `positive value`
* `custom_title`
	* Sets a custom title for the card.
* `disable_animations`
	* Disables animations for the card.
* `hide_border`
	* If `true`, sets card's border as hidden.
		* `true` `false`
* `hide_rank`
	* If `true`, sets the rank as hidden.
		* `true` `false`
* `hide_title`
	* If `true`, sets card's title as hidden.
		* `true` `false`
* `icon_color`
	* Sets icon color.
		* `hex color code`
* `line_height`
	* Sets line height between text lines.
		* `positive value`
* `show_icons`
	* If `true`, sets icons as hidden.
		* `true` `false`
* `text_color`
	* Sets text color.
		* `hex color code`
* `theme`
	* Sets a preset collection of parameters related to customization options.
		* [`one of the avaliable themes`](https://github.com/anuraghazra/github-readme-stats/blob/master/themes/README.md#stats)
* `title_color`
	* Sets title color.
		* `hex color code`



***
***

* Previous: [2. GitHub-flavored Markdown](https://erlete.github.io/github-customization-guide/guides/markdown-guide.html)
* Next: [4. GitHub Actions](https://erlete.github.io/github-customization-guide/guides/actions-guide.html)
