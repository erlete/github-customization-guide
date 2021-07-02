---
title: "GitHub-flavored Markdown"
author: "Paulo Sánchez"
---

MarkDown language files (those with `.markdown` or `.md` extensions, such as `README.md`) have different structural elements that can be used to format text contained in them.

This is a brief summary of said elements, pointing out their components and providing with some basic examples. The objective of this document is to set down the bases for the elaboration of a decent `README.md` file for GitHub.

_Note: examples provided in this document are built upon three steps or phases: **structures** (illustrations of the generic version of every element), **raw examples** (structure syntax with real contents) and **processed examples** (contents of raw examples after formatting). These steps are represented in a table, yet this only works for [span (in-line) elements](https://daringfireball.net/projects/markdown/syntax#span) (since they can be inserted in said tables). For [block elements](https://daringfireball.net/projects/markdown/syntax#block), an independent "Processed Example" is provided below the table containing both the structure and raw example._

## Text Style Formatting

***

Type | Structure | Raw Example | Processed Example
---- | --------- | ----------- | -----------------
Italic | \*`<text>`\* | \*Italic text\* | *Italic text*
Bold | \*\*`<text>`\*\* | \*\*Bold text\*\* | **Bold text**
Strike through | \~\~`<text>`\~\~ | \~\~Strike through text\~\~ | ~~Strike through text~~

## Headers

***

Headers are preceded by the `#` symbol. Since there are different sizes of headers, a hierarchy can be established using multiple `#`:

Structure | Raw Example
--------- | -----------
\# `<text>` | \# Header 1
\## `<text>` | \## Header 2
\### `<text>` | \### Header 3
\#### `<text>` | \#### Header 4
\##### `<text>` | \##### Header 5
\###### `<text>` | \###### Header 6

_For the sake of this document's design, no processed examples are provided, but you can test them all by yourself, it is quite easy!_

## Lists

***

### Unordered Lists

Structure | Raw Example
--------- | -----------
\* `1st level text`<br>    \* `2nd level text` | \* Main Element<br>    \* Nested Element

#### Processed Example:

* Main Element
  * Nested Element

### Ordered Lists

Structure | Raw Example
--------- | -----------
0\. `1st level text`<br>    1\. `2nd level text` | 0\. Main Element<br>    1\. Nested Element

#### Processed Example:

0. Main Element
   1. Nested Element

_Note: index numbers do not necessarily have to be ordered, since at the time of processing the contents of the list, those numbers are overwritten with procedurally generated values of a succession. The only thing that matters is that the ordered list is indexed as a collection of values followed by a dot._

## Links

***

### Normal Links

Links can be either direct (showing the links as text and setting them as clickable elements) or indirect (with clickable placeholders).

Type | Structure | Raw Example | Processed Example
---- | --------- | ----------- | -----------------
Direct | `<link>` | http://github.com | http://github.com
Indirect | \[`<placeholder>`\](`<link>`) | \[GitHub\]\(http://github.com) | [GitHub](http://github.com)

### Image Links

Image links are just normal indirect links with a preceding `!` symbol. This processes the image and embeds it in the document.

Structure | Raw Example
--------- | -----------
\!\[`<placeholder>`\](`<link>`) | \[GitHub Logo\](https://github.githubassets.com/images/modules/logos_page/GitHub-Logo.png)

#### Processed Example:

![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Logo.png)

### Image Links: Resizing

An alternative for easy image resizing is to use the `<img>` tag from HTML, to which the `src` (source), `alt` (alternative text or description), 
`width` and `height` parameters ([and many others](https://www.w3schools.com/tags/tag_img.asp)) can be passed. All those parameters' values must be enclosed in double quotes:

Structure | Raw Example
--------- | -----------
\<img src=`<link>` alt=`<text>` width=`<value>`> | \<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Logo.png" alt\="GitHub Logo" width\="25%">

#### Processed Example:

<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Logo.png" alt="GitHub Logo" width="25%">

## Blockquotes

***

These elements can be used to cite explicit fragments of some text extracted from another site. Their structure is as follows:

Structure | Raw Example
--------- | -----------
\> `<content>` | \> GitHub: Where the world builds software.

#### Processed Example:

> GitHub: Where the world builds software.

## Code

***

### Span (Plain)

Span code can be inserted into the document using single backticks (\` \`):

Structure | Raw Example | Processed
--------- | ----------- | -----------------
\``<code>`\` | \`#import <iostream>\` | `#import <iostream>`

### Block (Highlighted)

Block code can be inserted into the document using triple backticks (\`\`\` \`\`\`):

Structure | Raw Example
--------- | -----------
\`\`\``<language>`<br>`<code>`<br>\`\`\` | \`\`\`c++<br>#import \<iostream\><br>\`\`\`

#### Processed Example:

```c++
#import <iostream>
```

## Tables
 
 ***

Structure | Raw Example
--------- | -----------
`<Column 1 Header>` \| `<Column 2 Header>`<br>------------------- \| -------------------<br>`<Row 1 Column 1 Content>` \| `<Row 1 Column 2 Content>`<br>`<Row 2 Column 1 Content>` \| `<Row 2 Column 2 Content>` | Element \| Type<br>-------- \| -----<br>Link \| Span<br>Table \| Block

#### Processed Example:

Element | Type
------- | ----
Link | Span
Table | Block

## Task lists
 
 ***

Structure | Raw Example
--------- | -----------
\- \[  \] `<text>`<br>\- \[x\] `<text>` | \- \[  \] Pending Task<br>\- \[x\] Completed Task

#### Processed Example:

- [ ] Pending Task
- [x] Completed Task
