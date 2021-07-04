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

The structure of the above graph consists in a link referring to a server-hosted API that fetches your GitHub stats and displays them: 

`https://github-readme-stats.vercel.app/api`.

The content of said link can be displayed in your own README.md files using the [syntax for embedding images in markdown](https://erlete.github.io/github-customization-guide/guides/markdown-guide.html#image-links):

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

***

### Parameters

In this section there are two main indexes, ordered by [alphabetical order of the parameters](https://erlete.github.io/github-customization-guide/guides/stats-guide-1.html#alphabetical-order) and [parameters' area of application](https://erlete.github.io/github-customization-guide/guides/stats-guide-1.html#area-of-application). These indexes follow a specific structure:

* `Parameter identifier (name)`
	* Brief usage description
		* `Generic value structure`

***

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
		* `true` \| `false`
* `custom_title`
	* Sets a custom title for the card.
		* `text`
* `disable_animations`
	* Disables animations for the card.
		* `true` \| `false`
* `hide`
	* Takes one or many values and hides specific stats from the card.
		* `stars` \| `commits` \| `prs` \| `issues` \| `contribs`
* `hide_border`
	* If `true`, sets card's border as hidden.
		* `true` \| `false`
* `hide_rank`
	* If `true`, sets the rank as hidden.
		* `true` \| `false`
* `hide_title`
	* If `true`, sets card's title as hidden.
		* `true` \| `false`
* `icon_color`
	* Sets icon color.
		* `hexadecimal color code`
* `include_all_commits`
	* If `true`, all performed commits are counted.
		* `true` \| `false`
* `line_height`
	* Sets line height between text lines.
		* `positive value`
* `locale`
	* Sets card's language.
		* `language-1,language-2,...`
* `show_icons`
	* If `true`, sets icons as hidden.
		* `true` \| `false`
* `text_color`
	* Sets text color.
		* `hexadecimal color code`
* `theme`
	* Sets a preset collection of parameters related to customization options.
		* [`one of the avaliable themes`](https://github.com/anuraghazra/github-readme-stats/blob/master/themes/README.md#stats)
* `title_color`
	* Sets title color.
		* `hexadecimal color code`
* `show_owner`
	* If `true`, displays the name of the owner.
		* `true` \| `false`

***

#### Area of application

Since this index is divided in sections, this index might help you get a clear view of its contents:

* Background: background settings.
* Border: border settings.
* Contents: card's text and shape settings.
* Data Fetching: different data types' display and fetching.
* General Settings: themes and animations.
* Icons: icon settings.
* Title: title settings.

***

##### Background

* `bg_color`
	* Sets card's background color or [gradient].
		* `hexadecimal color code`

##### Border

* `border_color`
	* Sets border color.
		* `hexadecimal color code`
* `border_radius`
	* Sets border radius.
		* `positive value`
* `hide_border`
	* If `true`, sets card's border as hidden.
	* This setting cancels `border_radius` and `border_color` parameters.
		* `true` \| `false`

##### Contents

* `text_color`
	* Sets text color.
		* `hexadecimal color code`
* `line_height`
	* Sets line height between text lines.
		* `positive value`
* `locale`
	* Sets card's language.
		* `language-1,language-2,...`

##### Data Fetching

* `show_owner`
	* If `true`, displays the name of the owner.
		* `true` \| `false`
* `count_private`
	* If `true`, stats from private repositories are also gathered.
		* `true` \| `false`
* `include_all_commits`
	* If `true`, all performed commits are counted.
		* `true` \| `false`
* `hide`
	* Takes one or many values and hides specific stats from the card.
		* `stars` \| `commits` \| `prs` \| `issues` \| `contribs`
* `hide_rank`
	* If `true`, sets the rank as hidden.
		* `true` \| `false`
* `cache_seconds`
	* Sets the cache header manually.
		* `value from 1800 to 86400`

##### General Settings

* `theme`
	* Sets a preset collection of parameters related to customization options.
		* [`one of the avaliable themes`](https://github.com/anuraghazra/github-readme-stats/blob/master/themes/README.md#stats)
* `disable_animations`
	* Disables animations for the card.
		* `true` \| `false`

##### Icons

* `show_icons`
	* If `true`, sets icons as hidden.
		* `true` \| `false`
* `icon_color`
	* Sets icon color.
		* `hexadecimal color code`

##### Title

* `custom_title`
	* Sets a custom title for the card.
		* `text`
* `title_color`
	* Sets title color.
		* `hexadecimal color code`
* `hide_title`
	* If `true`, sets card's title as hidden.
	* This setting cancels `custom_title` parameter.
		* `true` \| `false`

***

## GitHub Language Cards

A language card able to display up to 10 language usage percentages.

![Erlete's GitHub languages](https://github-readme-stats.vercel.app/api/top-langs/?username=erlete)

***

As in GitHub stats cards, the top languages card is embedded in the document using a link:

`https://github-readme-stats.vercel.app/api/top-langs/`

The link takes a `username` parameter as well:

`https://github-readme-stats.vercel.app/api/top-langs/?username=<your username>`

In my case, the link looks like this:

`https://github-readme-stats.vercel.app/api/top-langs/?username=erlete`

However, the link takes customization parameters too, which are mentioned in the indexes below.

***

### Parameters

***

#### Alphabetical order

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
* `card_width`
	* Set card's width.
		* `positive value`
* `custom_title`
	* Sets a custom title for the card.
		* `text`
* `disable_animations`
	* Disables animations for the card.
		* `true` \| `false`
* `exclude_repo`
	* Exclude specified repositories from being scanned.
		* `repository-1,repository-2,...`
* `hide`
	* Hide the languages specified from the card.
	* This setting cancels (partially or totally) `langs_count` parameter.
		* `language-1,language-2,...`
* `hide_border`
	* If `true`, sets card's border as hidden.
	* This setting cancels `border_radius` and `border_color` parameters.
		* `true` \| `false`
* `hide_title`
	* If `true`, sets card's title as hidden.
	* This setting cancels `custom_title` parameter.
		* `true` \| `false`
* `icon_color`
	* Sets icon color.
		* `hexadecimal color code`
* `langs_count`
	* Sets the amount of languages shown in the card.
		* `value from 1 to 10`
* `layout`
	* Set card's layout.
		* `default` \| `compact`
* `line_height`
	* Sets line height between text lines.
		* `positive value`
* `locale`
	* Sets card's language.
		* `language-1,language-2,...`
* `show_icons`
	* If `true`, sets icons as hidden.
		* `true` \| `false`
* `text_color`
	* Sets text color.
		* `hexadecimal color code`
* `theme`
	* Sets a preset collection of parameters related to customization options.
		* [`one of the avaliable themes`](https://github.com/anuraghazra/github-readme-stats/blob/master/themes/README.md#stats)
* `title_color`
	* Sets title color.
		* `hexadecimal color code`

***

#### Area of application

Since this index is divided in sections, this index might help you get a clear view of its contents:

* Background: background settings.
* Border: border settings.
* Contents: card's text and shape settings.
* Data Fetching: different data types' display and fetching.
* General Settings: themes and animations.
* Icons: icon settings.
* Title: title settings.

***

##### Background

* `bg_color`
	* Sets card's background color or [gradient].
		* `hexadecimal color code`

##### Border

* `border_color`
	* Sets border color.
		* `hexadecimal color code`
* `border_radius`
	* Sets border radius.
		* `positive value`
* `hide_border`
	* If `true`, sets card's border as hidden.
	* This setting cancels `border_radius` and `border_color` parameters.
		* `true` \| `false`

##### Contents

* `text_color`
	* Sets text color.
		* `hexadecimal color code`
* `line_height`
	* Sets line height between text lines.
		* `positive value`
* `locale`
	* Sets card's language.
		* `language-1,language-2,...`
* `card_width`
	* Set card's width.
		* `positive value`
* `layout`
	* Set card's layout.
		* `default` \| `compact`

##### Data Fetching

* `langs_count`
	* Sets the amount of languages shown in the card.
		* `value from 1 to 10`
* `exclude_repo`
	* Exclude specified repositories from being scanned.
		* `repository-1,repository-2,...`
* `hide`
	* Hide the languages specified from the card.
	* This setting cancels (partially or totally) `langs_count` parameter.
		* `language-1,language-2,...`
* `cache_seconds`
	* Sets the cache header manually.
		* `value from 1800 to 86400`

##### General Settings

* `theme`
	* Sets a preset collection of parameters related to customization options.
		* [`one of the avaliable themes`](https://github.com/anuraghazra/github-readme-stats/blob/master/themes/README.md#stats)
* `disable_animations`
	* Disables animations for the card.
		* `true` \| `false`

##### Icons

* `show_icons`
	* If `true`, sets icons as hidden.
		* `true` \| `false`
* `icon_color`
	* Sets icon color.
		* `hexadecimal color code`

##### Title

* `custom_title`
	* Sets a custom title for the card.
		* `text`
* `title_color`
	* Sets title color.
		* `hexadecimal color code`
* `hide_title`
	* If `true`, sets card's title as hidden.
	* This setting cancels `custom_title` parameter.
		* `true` \| `false`

***

Previous: [2. GitHub-flavored Markdown](https://erlete.github.io/github-customization-guide/guides/markdown-guide.html) | Next: [4. GitHub Actions](https://erlete.github.io/github-customization-guide/guides/actions-guide.html)
