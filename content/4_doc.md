---
title: Preparing Your Document
nav: Preparing Your Document
gallery: true
---

{% include feature/nav-menu.html sections="Header Material;Formatting Example;Styling" %}

<br>

{% include feature/button.html text="Make a Copy of the Doc Template to Begin" link="https://docs.google.com/document/d/1eQeySiAK-4O-e6Ym5lIRsNloiFa6IFg15qdthnaFLwo/copy" color="success" size="lg" centered="true" %}

<br>

## Header Material

<br>

> Once you have your copy, rename your file using this pattern= `(last name)_(first name)_doc`. 

Next, adjust your header material at the top of the Doc template. Depending on the course, this may be as simple as entering the name of the essay after the title field and adding your author name, or it may include more detailed metadata like location and theme of your research subject. Check your syllabus to see what metadata fields might be unique to your project, or if they are using a standardized language they want you to assign to your project, such as:
> `gender; sexuality; labor; inequality; spectacle; violence`, as examples you might include for theme. 

{% include alert.html text="**Note**: If needed, a simple way to record the latitude and longitude of your research subject is to visit [Google Maps](https://www.google.com/maps). Selecting any area with the right mouse key will bring up those coordinates at the top of the dropdown menu that appears. Selecting the coordinates will automatically copy the data to your clipboard." color="light" align="left" %}  

**Example**

```
—
Title: Development of the Wallace, Idaho Mining Industry
Author(s): Hillary Hecla; Bill Bunker
Location: Wallace, Idaho
Lat/Long: 47.47502530031415; -115.92450766818784
—
```

{% include alert.html text="**Note**: If you have multiple values, like two, authors, coordinates or themes, separate them with a semi-colon: **;**" color="light" align="left" %}  

<br>

## Formatting Example

<br>

Fill in your essay as you would normally, but indicate where you would like your media to appear by creating a break, followed by: (objectid: "objectid name"). For example:

<br>

```

# Title

Body 1 with image example

(objectid:mining_01)

## Subheading (if needed)

Body 2 with PDF example

(objectid:mining_02)

Body 3 with video embed example

(objectid:mining_03)

```

> would look like:

# Title

Body 1 with image example

{% include gallery-figure.html img="mining_01.jpg" alt="The caption describes everything that is not in the image, like date, location and people's names, whereas alternate text describes everything that is in the image, so it is accessible. An example for this image might be: A long, industrial wooden building constructed on the side of a hill with shacks in the fore and background." caption="The metadata you provide in your sheets provides caption material. Select the image to see the alternate text along the bottom of the image." width="75%" %}

## Subheading (if needed)

Body 2 with PDF example

{% include feature/pdf.html objectid="https://objects.lib.uidaho.edu/bigburn/bigburn02.pdf" %}

Body 3 with video embed example
 
{% include feature/video.html objectid="https://www.youtube.com/watch?v=gWKiBKlZV88" %}

<br>

### Styling

<br>

Add your styling as you normally would to a Google doc, including _italics_, **bolded words**, 

- lists, 

---

line breaks 

and 

> block quotes

But note that when we convert your Doc into a markdown file, it will look like the section on the left:

<br>

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

Headings aren't just decorative, they are _hierarchical_. This means that the different headings you use dictate how a page is navigated by people using a keyboard or screen readers. 

> Start with `heading one` for your title, then go down incrementally for subheadings if needed.

<br>