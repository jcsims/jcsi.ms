+++
comments = false
draft = false
categories = ["markdown"]
date = "2012-10-31T00:00:00-07:00"
title = "Markdown Cheatsheet"
slug = "markdown-cheatsheet"
tags = []
+++

This is a short post documenting the common items I use in Markdown.  This
information is pulled from John Gruber's original [documentation][doc].

[doc]: http://daringfireball.net/projects/markdown/syntax

- [Paragraphs](#Paragraphs)
- [Headings](#Headings)
- [Lists](#Lists)
- [Blockquotes](#Blockquotes)
- [Code Block](#Code_Block)
- [Horizontal Rule](#Horizontal_Rule)
- [Links](#Links)
- [Images](#Images)
- [Emphasis](#Emphasis)



<a id="Paragraphs"> </a>

## Paragraphs

Paragraphs are simply text seperated by at least one "empty" line - "empty"
meaning that there are either no characters or just whitespace characters on a
line.

    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
    consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
    cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
    proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
    consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
    cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
    proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

<a id="Headings"> </a>

## Headings

Headings are fairly simple:

    # Heading 1
    ## Heading 2
    ### Heading 3
    #### Heading 4

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

<a id="Lists"> </a>

## Lists

### Bullet Lists

Bullet lists can use any of `*`, `-` or `+` to create bullets:

    * Item 1
    * Item 2
    - Item 3
    + Item 4

* Item 1
* Item 2
- Item 3
+ Item 4

### Numbered lists

Numbered lists simly have to have numbers in front of them, not necessarily in
order:

    1. apples
    3. bananas
    7. oranges
    7. potatoes

1. apples
3. bananas
7. oranges
7. potatoes

<a id="Blockquotes"> </a>

## Blockquotes

Blockquotes are typically used for emphasis.

    >"Any intelligent fool can make things bigger, more complex, and more
    > violent. It takes a touch of genius -- and a lot of courage -- to move
    > in the opposite direction."
    >
    > -Albert Einstein

>"Any intelligent fool can make things bigger, more complex, and more
> violent. It takes a touch of genius -- and a lot of courage -- to move
> in the opposite direction."
>
> -Albert Einstein

<a id="Code_Block"> </a>

## Code Block

To show some form of text without any kind of processing (typically code), use
a code block:  this is done by indenting the text 4 spaces.  All the examples
on this page use this.

<a id="Horizontal_Rule"> </a>

## Horizontal Rule

A horizontal rule is just a line used to break up the page.  It's made by three
or more underscores, hyphens, or asterisks:

    ___
    ---
    * * *

___
---
* * *

<a id="Links"> </a>

## Links

Links can be defined in two ways: inline or by reference.  The reference
definition can be anywhere in the document, as long as it's on it's own line.
I usually prefer to collect them at the bottom for easier editing.

    This is an [inline](https://www.google.com) link.

    This is a [reference][ref] link.

    [ref]: https://google.com

This is an [inline](https://www.google.com) link.

This is a [reference][ref] link.

[ref]: https://google.com

<a id="Images"> </a>

## Images

Linking images is very similar to creating regular [links](#Links), but with
one small change- add an excalamation point before the link.  Images can be
linked by both inline and reference methods.

    ![fat cat](https://dl.dropbox.com/u/2707922/2012-10-31%2019.28.19.jpg)

![fat cat](https://dl.dropbox.com/u/2707922/2012-10-31%2019.28.19.jpg)


<a id="Emphasis"> </a>

## Emphasis

Emphasis in the text is created with surrounding words or sentences with either
an asterisk or underscore.  Stronger emphasis can be created with double asterisk
or underscore:

    _Whoa!_

    That was a *huge* shark.

    That was **really** close!

_Whoa!_

That was a *huge* shark.

That was **really** close!
