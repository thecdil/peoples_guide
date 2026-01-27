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

## Essay Content

<br>

Write your essay content as normal below the header area. 
Try to keep any formatting simple since this content will become a webpage where text reflows to many different screen sizes--any complex formatting or layout in the Doc will be stripped away when converting into data (Markdown) for the project.
Feel free to use inline styles such as _italics_ and **bold**, and block styles such as lists and block quotes.

### Headings

While writing for the web, you will want to use a lot of headings (those bolded phrases breaking up the text like "Headings" above this line). 
When reading on the web, users expect more headings than a typical academic essay.
They function to help people navigate and understand your content--think of them like a table of contents, dividing the text into logical sections and sub-sections.

To apply headings in your Google Doc, select the text that should be a heading, then in the menu ribbon above, select the dropdown that says "Normal text" and change it to "Heading 1", "Heading 2", etc. 
Your headings are _hierarchical_ and should follow in logical order, starting from "Heading 1" and increasing sequentially (with out skipping levels) for sub-topics.
When you start a new topic, you can jump back up the levels to reflect the structure of your content.

### Images and Media 

Rather than pasting images or other media directly into your document, you will use a basic convention. 
First, you will fill in the individual image's information in your Item metadata spreadsheet (details in the next section). 
Then, in the location in your text where you would like images or other media to appear, add a blank line, then put `[objectid: <objectid>]` where "<objectid>" matches the id from your item metadata spreadsheet. 

When your essay is converted into data for the website project, this convention will pull in the information from your metadata spreadsheet to add the image to the web page. 
This ensures that each media Item is fully documented as a source and correctly formatted for the web.

For example, using the convention: 

`[objectid: mining_01]`

on the final website might be displayed like:

{% include gallery-figure.html img="mining_01.jpg" alt="The caption describes everything that is not in the image, like date, location and people's names, whereas alternate text describes everything that is in the image, so it is accessible. An example for this image might be: A long, industrial wooden building constructed on the side of a hill with shacks in the fore and background." caption="The metadata you provide in your sheets provides caption material. Select the image to see the alternate text along the bottom of the image." width="75%" %}

A YouTube video would like like:

`[objectid: mining_03]`
 
{% include feature/video.html objectid="https://www.youtube.com/watch?v=gWKiBKlZV88" %}
