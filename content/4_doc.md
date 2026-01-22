---
title: Preparing Your Document
nav: Preparing Your Document
gallery: true
---

{% include feature/nav-menu.html sections="Header Material;Markdown Basics;Headings;Paragraphs;Lists;Inline Elements;Code;Tables;Block Quotes;Horizontal Rule;Comments" %}

<br>

{% include feature/button.html text="Make a Copy of the Doc Template" link="https://docs.google.com/document/d/1eQeySiAK-4O-e6Ym5lIRsNloiFa6IFg15qdthnaFLwo/copy" color="success" size="lg" centered="true" %}

<br>

## Header Material

<br>

Once you have your copy, rename your file using this pattern= (last name)_(first name)_doc. Next, adjust your header material at the top of the Doc template. Depending on the course, this may be as simple as entering the name of the essay after the title field and adding you author name, or it may include more detailed metadata like location and theme of your research subject. Check your syllabus to see what metadata fields might be unique to your project, or if they are using a standardized language they want you to assign to your project, such as `gender;sexualitylabor
inequality
spectacle
violence

{% include alert.html text="Note: If needed, a simple way to record the latitude and longitude of your research subject is to visit [Google Maps](https://www.google.com/maps). Selecting any area with the right mouse key will bring up those coordinates at the top of the dropdown menu that appears. Selecting the coordinates will automatically copy the data to your clipboard." color="light" align="left" %}  

**Example**

```
—
Title: Development of the Wallace, Idaho Mining Industry
Author(s): Hillary Hecla; Bill Bunker
Location: Wallace, Idaho
Lat/Long: 47.47502530031415, -115.92450766818784
—
```

<br>

## Markdown Basics

<br>

### Headings 

<br>

Headings range from level one to six, with one being the most important concepts.
They should generally move up in order without skipping a level.

Be sure to include a blank line above and below a heading.

{% capture atxtext %}
<div class="row">
<div class="col-md-6" markdown="1">
```
# Heading One

## Heading Two

### Heading Three
```
</div>
<div class="col-md-6 md-demo" markdown="1">
# Heading One

## Heading Two

### Heading Three
</div>
</div>
{% endcapture %}
{% include card.html text=atxtext %}

<br>

### Paragraphs 

<br>

Paragraphs don't require any special markup.
Just leave an empty line between your paragraphs and any other block element.
For example:

{% capture par %}
```
Any text with no empty lines between will be joined into a paragraph.
Leave an empty line between headings and paragraphs.

Since there is an empty line above, 
this will start a new paragraph.
This gives you the option to write a paragraph all on one line 
(like a word processor),
or to put each sentence on its own line.
Splitting the sentences can make editing and version control easier. 
```

----------------

Any text with no empty lines between will be joined into a paragraph.
Leave an empty line between headings and paragraphs.

Since there is an empty line above, 
this will start a new paragraph.
This gives you the option to write a paragraph all on one line 
(like a word processor),
or to put each sentence on its own line.
Splitting the sentences can make editing and version control easier. 
{% endcapture %}
{% include card.html text=par %}

<br>

### Lists

<br>

A bullet list (i.e. **unordered list**) is created using `-` followed by a space (alternatively can use `*` or `+`).
Put each list item on a new line.
A numbered list (i.e. **ordered list**) is created using a number + `.` followed by a space.
The items will be automatically renumbered correctly in outputs. 
Both kinds of lists can be nested by tabbing in a level.

{% capture lists %}
<div class="row">
<div class="col-md-6" markdown="1">
```
- dog
- cat
- muffin
```
</div>
<div class="col-md-6 md-demo" markdown="1">
- dog
- cat
- muffin
</div>
</div>
<hr>
<div class="row">
<div class="col-md-6" markdown="1">
```
1. dog
2. cat
6. muffin
1. other thing
```
</div>
<div class="col-md-6 md-demo" markdown="1">
1. dog
2. cat
6. muffin
1. other thing
</div>
</div>
<hr>
<div class="row">
<div class="col-md-6" markdown="1">
```
1. dog
    - bark
    - wag
2. cat
    - meow
6. muffin
    - yum
```
</div>
<div class="col-md-6 md-demo" markdown="1">
1. dog
    - bark
    - wag
2. cat
    - meow
6. muffin
    - yum
</div>
</div>

------

Note, many platforms will also support to-do lists following the pattern: 

```
- [ ] task one
- [x] completed task
```

{% endcapture %}
{% include card.html text=lists %}

<br>

### Inline Elements

<br>

{% capture inline %}
<div class="row">
<div class="col-md-6" markdown="1">
```
*Emphasis* or _emphasis_

**Strong** or __strong__

**_Strong and Emphasis_**
```
</div>
<div class="col-md-6 md-demo" markdown="1">
*Emphasis* or _emphasis_

**Strong** or __strong__

**_Strong and Emphasis_**
</div>
</div>
<hr>

```
[hyperlink](https://www.google.com)

image: 

![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png)
```

[hyperlink](https://www.google.com)

image: 

![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png)

--------

```
example footnote.[^1]

[^1]: footnote definition will show up at bottom.
```

example footnote.[^1]

[^1]: footnote definition will show up at bottom.

{% endcapture %}
{% include card.html text=inline %}

<br>

### Code 

<br>

{% capture code %}

    Code can be highlighted inline with `backticks`.

    {% raw %}```{% endraw %}
    Or make a code block 
    open with three backticks alone on a line 
    and close with three more on a line. 
    {% raw %}```{% endraw %}

    This makes it easier to copy unformatted code/text

----------------

Code can be highlighted inline with `backticks`.

```
Or make a code block 
open with three backticks alone on a line 
and close with three more on a line. 
```

This makes it easier to copy unformatted code/text

{% endcapture %}
{% include card.html text=code %}

<br>

### Tables 

<br>

Tables aren't supported by all Markdown converters, but can be useful for some quick structure.

{% capture table %}

```
| column1 | column2 | column3 |
| --- | --- | --- |
| value | value | value |
| value | value | value |

```

-----------

{:.table .table-bordered}
| column1 | column2 | column3 |
| --- | --- | --- |
| value | value | value |
| value | value | value |

{% endcapture %}
{% include card.html text=table %}

<br>

### Block Quotes

<br>

{% capture bq %}
```
> Each line starts with greater-than space.
> Any other markdown can be used.
```

-------

> Each line starts with greater-than space.
> Any other markdown can be used.

{% endcapture %}
{% include card.html text=bq %}

<br>

### Horizontal Rule 

<br>

{% capture hr %}

```
Three or more dashes on a line:

----

```

Three or more dashes on a line:

----

{% endcapture %}
{% include card.html text=hr %}

<br>

### Comments 

<br>

`<!-- you can use HTML comments, they won't show up -->`

<br>

{% include alert.html text="Although Markdown is simple, it is important to remember that white space, blank lines, and tabs matter. 
If you are getting unexpected results when rendering, check your white space!" color="light" %}


<br>