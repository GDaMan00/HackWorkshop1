# Learn Frontend Workshop

In this workshop, we are going to teach you common components front-end developers typically build for websites. You can use this document as reference material for HTML and CSS.

## HTML Documentation

HTML stands for HyperText Markup Language. It is a markup language that enables us to write web pages using code to indicate how text and data should be displayed. HTML files also end with the extension ".html".

### HTML Template

Below is the common HTML structure

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    ....content of webpage.....
</body>
</html>
```

### Common HTML Elements/Tags

* **<!DOCTYPE>** - Defines the document type
* **\<html>** - Defines an HTML document
* **\<head>** - Defines information about the document
* **\<title>** - Defines a title for the document
* **\<body>** - Defines the document's body
* **\<h1> to \<h6>** - Defines HTML headings
* **\<p>** - Defines a paragraph
* **\<br/>** - Inserts a single line break
* **\<!--...-->** - Defines a comment
* **\<ul>** - Defines a container for an unordered list
* **\<ol>** - Defines a container for an ordered list
* **\<li>** - Defines a single list items
* **\<a href="">** - Defines a hyperlink, which is used to link from one page to another. Href indicates the link's destination.
A step by step series of examples that tell you how to get a development env running
* **\<img src="" alt="">** - Defines an image from the src value and gives alternative based on alt value
* **\<div>** - Defines a container for elements
* **\<section>** - Defines a container for elements
* **\<span>** - Defines an inline container for elements(doesn't go to new line)

Example of tag usage
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    <!-- This is a comment -->
    <h1>This is a title tag</h1>
    <p>This is a paragraph tag</p>
    <p>example of <br>tag</p>
    <ul>
        <li>one</li>
        <li>Two</li>
    </ul>
    <ol>
        <li>one</li>
        <li>Two</li>
    </ol>
    <a href="path/to/file">link</a>
    <img src="path/to/file" alt="image alternative">
    <div>
        example of using div<span>example of span</span>     
    </div>
    <section>example of section</section>
</body>
</html>
```
### Ids vs. Classes
Ids are used to uniquely identify one element on the page while classes can be used to identify more than one element.

ID example

```
<div id="example">Some text</div>
```

Class example

```
<div class="example">Some text</div>
```

## CSS Documentation

CSS (Cascading Style Sheets) is a language which specifies a page’s appearance. CSS does this by selecting an element within the HTML and styling it.

### How to Select Elements with CSS

Template of how css selects elements

```
/* the selector is used to target an element on a page. */
selector { property: value; /* more properties...*/ }
```

Examples of selecting elements
```
/* Selecting by class */
.class1 { }

/* Selecting by name */
div { }

/* Selecting by id */
#anID { }

/* Selecting by attribute */
[attr] { font-size:smaller; }

/* Selecting by an attribute's value */
[attr='value'] { font-size:smaller; }

/* Selecting the child of another element */
div.some-parent > .class-name { }

/* Selecting descendant of another element */
div.some-parent .class-name { }

/* Selecting by adjacent siblings */
.i-am-just-before + .this-element { }

/* Selecting by preceding elements */
.i-am-any-element-before ~ .this-element { }

```

### CSS Order of Precedence

In CSS, selectors can override other selectors based on specificity

Specificity Rule (Most to Least)

1 Inline styles - styling the HTML directly on the HTML element

```
<div style="background-color: red;">Inline Styling</div>
```

2 IDS
```
#id {background-color: red;}
```

3 Classes
```
.class {background-color: red;}
```

4 Elements
```
div {background-color: red;}
```

### Box Model
The CSS box model is the box that wraps every single HTML element. This model consists of all of the visual formatting elements, such as border, padding, border-radius, and content.The details of the box model will be covered in the section below.

```
.sample{
    /* "width" specifies the width of the elements and can be in a variety of units (i.e. em, rem, px, %)
    width: 100%;

    /* "height" specifies the height of the elements and can be in a variety of units (i.e. em, rem, px, %)
    height: 250px;
    
    /* "margin" specifies the spacing between the selected element's box and neighboring elements */
    margin: 1em;
    
    /* "padding" specifies the spacing between the content inside of an element's box and the edge of the box */
    padding: 20px;

    /* "border" specifies the styling of the edge of the box content */
    border: 5px solid red;
}
```

### Visual Formatting: Dimensions, Display, and Positioning
One of CSS's main roles is to format the content that is specified by the HTML. It performs formatting tasks using a variety of formatting attributes defined below.

```
.sample{

    /* "display" specifies the display of the elements */
    display: flex; 
    
    /* "position" specifies the type of positioning that should be used by an element */
    position: relative;
    
    /* "top" specifies how far the content is relative to something else */
    top: 20px;

    /* "bottom" specifies how far the content is relative to something else */
    bottom: 20px;

    /* "left" specifies how far the content is relative to something else */
    left: 20px;

    /* "right" specifies how far the content is relative to something else */
    right: 20px;
}
```

#### Flexbox
The Flexible Box, otherwise known as flexbox, offers simple yet powerful capabilities in aligning content on a page. We will be using this technique in the tutorial to layout content for the navigation bar and cards. Listed below are the common attributes of flexbox.

```
.sample{
 
    /* Setting the "display" to "flex" allows the selected element to be a flexbox and use flexbox attributes */
    display: flex;
        
    /* Using the "flex-direction" attribute sets the direction of alignment for the elements within the flexbox */
    flex-direction: row; /* Can also be row, column, column-reverse, row-reverse */
        
    /* Using the "justify-content" attribute aligns the content along the main axis, which is defined by the flex-direction */
    justify-content: center; /* Can also be flex-start, flex-end, etc. */
        
    /* Using the "align-items" attribute aligns the content along the perpendicular of the main axis */
    align-items: center; /* Can also be flex-start, flex-end, etc. */
        
    /* Using the "flex-wrap" property wraps elements when they exceed the boundaries of the parent box */
    flex-wrap: wrap;   
}
```

### Colors and Backgrounds
A page without colors can be bland. Therefore, being able to style the color of a page is an important characteristic of CSS. The two main types of color styling are demonstrated below.

```
.sample{
        
    /* "color" sets the color of the text for the elements it is applied to */
    color: purple;
        
    /* "background" sets the color of the background, which is the rest of the box that is not the content */
    background: gray;
        
}
```

### Text and Fonts
CSS can also be used to style and align textual content so that you can style content without styling the entire element box itself 

```
.sample{
        
    /* "text-align" aligns the content within its enclosing element */
    text-align: center; /* Can also be left, right, etc. */
    
    /* "font-family" defines the font that is used for an element
    font-family: sans-serif;
        
    /* "font-size" defines the size that textual content should be in an element */
    font-size: 2rem; /* Follows the same unit standards as defined above */
    
}
```

## Other Resources

Reference Materials
* W3 Schools HTML (https://www.w3schools.com/html/) - Reference for HTML
* W3 Schools CSS (https://www.w3schools.com/css/) - Reference for CSS
* W3 Schools JS (https://www.w3schools.com/js/) - Reference for JS
* CSS Tricks (https://css-tricks.com/) - Helpful tutorials for CSS
* Tutorials Point (https://www.tutorialspoint.com/) - Overall programming reference material
* Learn HTML in Y minutes (https://learnxinyminutes.com/docs/html/) - Fast guide on html
* Learn CSS in Y minutes (https://learnxinyminutes.com/docs/css/) - Fast guide on css
* Flexbox Docs - (https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Reference for flexbox

Learning Platforms
* Free Code Camp (https://www.freecodecamp.org/) - Front-end development learning platform
* Code Academy (https://www.codecademy.com/) - General programming learning platform (includes front-end development)
* Froggy (flexbox) (https://flexboxfroggy.com/) - Interactive flexbox tutorial

## Feedback
https://goo.gl/forms/nzQL6aU2f42E1gWz2 

