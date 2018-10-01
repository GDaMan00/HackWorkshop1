# Learn Frontend Workshop

In this workshop we are going to teach you common components frontend developers typically build out for a website. You can use this readme as a reference material for HTML and CSS.

## HTML DOCS

HTML stands for HyperText Markup Language. It is a language which allows us to write pages for the world wide web. It is a markup language, it enables us to write webpages using code to indicate how text and data should be displayed. HTML files also end with the extension .html like index.html or foo.html.

### HTML TEMPLATE

This is what the structure of an HTML Document look like

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

### Common HTML elements/tags

* **<!DOCTYPE>** 	Defines the document type
* **\<html>** - Defines an HTML document
* **\<head>** - Defines information about the document
* **\<title>** - Defines a title for the document
* **\<body>** - Defines the document's body
* **\<h1> to \<h6>** - Defines HTML headings
* **\<p>** - Defines a paragraph
* **\<br>** - Inserts a single line break
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

Example of using the tags
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
### IDS vs CLASSES
Ids are used to uniquely identify one element on the page while classes can be used to identify more than one element.

ID example

```
<div id="example">Some text</div>
```

Class example

```
<div class="example">Some text</div>
```

## CSS DOCS

CSS (Cascading Style Sheets) is a language which specifies a page’s appearance. CSS does this by selecting an element within the html and style it.

### How to select elements with css

Template of how css selects elements

```
/* the selector is used to target an element on a page. */
selector { property: value; /* more properties...*/ }
```

Examples of selecting elements
```
/* You can target it using one of its CSS classes */
.class1 { }

/* or its name */
div { }

/* or its id */
#anID { }

/* or using the fact that it has an attribute! */
[attr] { font-size:smaller; }

/* or that the attribute has a specific value */
[attr='value'] { font-size:smaller; }

/* You can select an element which is a child of another element */
div.some-parent > .class-name { }

/* or a descendant of another element. Children are the direct descendants of
   their parent element, only one level down the tree. Descendants can be any
   level down the tree. */
div.some-parent .class-name { }

/* You may also select an element based on its adjacent sibling */
.i-am-just-before + .this-element { }

/* or any sibling preceding it */
.i-am-any-element-before ~ .this-element { }

/* for example, when the cursor hovers over an element */
selector:hover { }
```

### CSS Order of Precedence

In css selectors can override other selectors based on specificity

Specificity Rule(Greatest to Least)

1 Inline styles - styling the html directly on the html element

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

## Box Model

## Visual Formatting: dimensions, display, and positioning

### Flexbox

## Colors and Backgrounds

## Text and Fonts



## Other Resources

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

