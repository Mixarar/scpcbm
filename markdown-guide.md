---
title: Markdown Guide
description: A comprehensive guide on markdown that is supported on our wiki.
published: true
date: 2023-10-16T20:24:40.548Z
tags: en
editor: markdown
dateCreated: 2023-10-15T16:53:41.075Z
---

# Embed images

## Embed images {.tabset}

### Preview
![image with 64x64 pixels](/images/roles/classd.png =64x)

The image is embedded directly ![image with 16x16 pixels](/images/roles/classd.png =16x) in the text.
The resolution is defined as `16x16 pixels` so that it fits well into the flow of the text.
Without optional dimension specification, the image would be presented in full resolution.

### Source code

```markdown
![image with 64x64 pixels](/barraco-512.jpg =64x)

The image is embedded directly ![image with 16x16 pixels](/barraco-512.jpg =16x) in the text.
The resolution is defined as `16x16 pixels` so that it fits well into the flow of the text.
Without optional dimension specification, the image would be presented in full resolution.
```

# Embed images (with spoiler)

## Embed images (with spoiler) {.tabset}

### Preview

<details>

![image as spoiler](/images/roles/classd.png =64x)

</details>

### Source code

```markdown
<details>

![image as spoiler](/images/roles/classd.png)


</details>
```

# block quote

## block quote {.tabset}

### Preview

> This is a regular block quote.

> This is a information block.
{.is-info}

> This is a success block.
{.is-success}

> This is a warning block.
{.is-warning}

> This is a error/danger block.
{.is-danger}

### Source code

```markdown
> This is a regular block quote.

> This is a information block.
{.is-info}

> This is a success block.
{.is-success}

> This is a warning block.
{.is-warning}

> This is a error/danger block.
{.is-danger}
```

# Emoji

## Emoji {.tabset}

### Preview

You can use a variety of emojis like :palm_tree: or :tea:.

### Source code

```markdown
You can use a variety of emojis like :palm_tree: or :tea:.
```

### Notes

> A detailed overview of supported emojis can be found in this [Cheat Sheet](https://www.webfx.com/tools/emoji-cheat-sheet/).
{.is info}

# footnotes

## footnotes {.tabset}

### Preview

In this text[^1] there are two footnotes[^2].
The footnotes can be found in the end of each page.

[^1]: This is the first footnote.
[^2]: This is the second footnote.

### Source code

```markdown
In this text[^1] there are two footnotes[^2].
The footnotes can be found in the end of each page.

[^1]: This is the first footnote.
[^2]: This is the second footnote.
```

# Horizontal dividing line

## Horizontal separator {.tabset}

### Preview

This text is separated with a horizontal line

---

separate dividing line.

### Source code

```markdown
This text is separated with a horizontal line

---

separate dividing line.
```

# hiperlinks

## Hiperlinks {.tabset}

### Preview

The hiperlinks can be embedded as [text](sintaxe/markdown) and as image [![image with 16x16 pixels](/images/roles/classd.png =16x)](sintaxe/markdown).

### Source code

```markdown
The hiperlinks can be embedded as [text](sintaxe/markdown) and as image [![image with 16x16 pixels](/images/roles/classd.png =16x)](sintaxe/markdown).
```

# list (todo list)

## list (todo list) {.tabset}

### Preview

- [X] This list entry is complete.
- [ ] This list entry has yet to be made.

### Source code

```markdown
- [X] This list entry is complete.
- [ ] This list entry has yet to be made.
```

# list (numbering)

## list (numbering) {.tabset}

### Preview

1. First entry
2. Second entry
3. Third entry

### Source code

```markdown
1. First entry
2. Second entry
3. Third entry
```

### Notes

> It's suficient numbering all entries with `1.`.
> When the page is built, the numbering is automatically corrected and counted in the recorded order.
{.is info}

# list (without numbering)

## lista (without numbering) {.tabset}

### Preview

Here is a example of a simple list:
- A simple list entry
- Yet another simple list entry
- And another simple list entry

Here is a example of a grid list:
- A grid element
- Another grid element
- And another grid element
{.grid-list}

Here is a example of a list formated especially for hyperlinks:
- [A hiperlink *with description*](sintaxe/markdown)
- [Another hiperlink *with aditional description*](sintaxe/markdown)
- [And another hiperlink *also with description*](sintaxe/markdown)
{.links-list}

### Source code

```markdown
Here is a example of a simple list:
- A simple list entry
- Yet another simple list entry
- And another simple list entry

Here is a example of a grid list:
- A grid element
- Another grid element
- And another grid element
{.grid-list}

Here is a example of a list formated especially for hyperlinks:
- [A hiperlink *with description*](sintaxe/markdown)
- [Another hiperlink *with aditional description*](sintaxe/markdown)
- [And another hiperlink *also with description*](sintaxe/markdown)
{.links-list}
```

# Source code

## Source code {.tabset}

### Preview

This text contains `inline` source code formatting.

```
This entire text block is formatted as source code.
```

Example with highlight:

```csharp
public static void Main(string[] args)
{
                 Ambiente.Exit(0);
}
```

### Source code

````markdown
This text contains `inline` source code formatting.

```
This entire text block is formatted as source code.
```

Example with highlight:

```csharp
public static void Main(string[] args)
{
                 Ambiente.Exit(0);
}
```
````

# spoilers

## spoilers {.tabset}

### Preview

<details>
   <summary>Warning: Spoilers</summary>
   This is a spoiler text.
</details>

### Source code

```markdown
<details>
   <summary>Warning: Spoilers</summary>
   This is a spoiler text.
</details>
```

# Table

## Table {.tabset}

### Preview

| Designation | type | value |
|:-------------- |:-------:| ----:|
| First element | First | 1600 |
| Second element | Second | 12 |
| Third element | Third | 1 |

### Source code

```markdown
| Designation | type | value |
|:-------------- |:-------:| ----:|
| First element | First | 1600 |
| Second element | Second | 12 |
| Third element | Third | 1 |
```

# tabs

## Tabs {.tabset}

### Preview

The tabs, which can already be seen on the whole page, should serve as an example.

### Source code

````markdown
## Tabs {.tabset}

### Preview

The tabs, which can already be seen on the whole page, should serve as an example.

### Source code

```markdown
TEXT...
```
````

### Notes

> The tabs can only be used if the corresponding titles are used.
> As can be seem in the example, the element `{.tabset}` must be attached to a top header.
> For each tab, a corresponding header must be specified one level below, which serves as a tab designation.
{.is-info}

# keyboard icons

## keyboard icons {.tabset}

### Preview

The keyboard icons can also be rendered to improve documentation and guides

<kbd>CTRL</kbd> + <kbd>X</kbd> to cut a content.
<kbd>CTRL</kbd> + <kbd>C</kbd> to copy a content.
<kbd>CTRL</kbd> + <kbd>V</kbd> to paste a content.

### Source code

```markdown
The keyboard icons can also be rendered to improve documentation and guides

<kbd>CTRL</kbd> + <kbd>X</kbd> to cut a content.
<kbd>CTRL</kbd> + <kbd>C</kbd> to copy a content.
<kbd>CTRL</kbd> + <kbd>V</kbd> to paste a content.
```

# Text formatting

## Text formatting {.tabset}

### Preview

This text is in **bold**.

This text is in *italic*.

This text is <ins>underlined</ins>.
This text is also <u>underlined</u>.

This text is ~~crossed out~~.

This text is ^superscript^.

This text is ~subscript~.

### Source code

```markdown
This text is in **bold**.

This text is in *italic*.

This text is <ins>underlined</ins>.
This text is also <u>underlined</u>.

This text is ~~crossed out~~.

This text is ^superscript^.

This text is ~subscript~.
```

### Key combination

<kbd>CTRL</kbd> + <kbd>B</kbd> for **bold**.
<kbd>CTRL</kbd> + <kbd>I</kbd> for *italic*.


# Headlines

## Titles {.tabset}

### Preview

The titles are also used very frequently in this page.

The level of the title can be specified using `#`. The fewer `#`, the higher the level and vice versa.
The syntax can be checked accordingly in the source text tab.

As alternative, `=` or `-` can also be inserted below the headline.

### Source code

```
# 1st level header
## 2nd level header
### 3rd level header
#### 4th level header
##### 5th level header
###### 6th level header

####### This is no longer a header.

This is an alternative syntax for a level 1 heading
==

This is an alternative syntax for a level 2 heading
--
```

# Additional

There are other functions that still must be documented or are provided by plugins.

> Wiki.js offers full markdown support.
> Therefore, functions not described here should also work (e.g. embedding YouTube videos, etc.).
{.is info}