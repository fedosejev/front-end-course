# Day 3

Questions:

1. [Why do we need web pages?](#why-do-we-need-web-pages)
2. [Why do we need documents to have structure?](#why-do-you-want-your-documents-to-have-structure)
3. [What structure would you choose for your documents?](#what-structure-would-you-choose-for-your-documents)
4. [How do we describe a tree structure of a document to a web browser?](#how-do-we-describe-a-tree-structure-of-a-document-to-a-web-browser)
5. [What is an HTML element?](#what-is-an-html-element)
6. [What are tag attributes?](#what-are-tag-attributes)
7. [What is the structure of a valid HTML document?](#what-is-the-structure-of-a-valid-html-document)
8. [How to valide my HTML document?](#how-to-valide-my-html-document)
9. [Why my whitespace is not displayed?](#why-my-whitespace-is-not-displayed)
10. [Which HTML tag should I choose?](#which-html-tag-should-i-choose)

Plus:

+ [Problems](problems.md)
+ [Learn more](#learn-more)

## Questions

### Why do we need web pages?

Think of how we organised and structured information before the Internet.

We represented information in a form of paper __documents__. (_Paper is a medium, just like a screen._)

Examples of documents in every day of our lives:
+ Newspapers
+ Magazines
+ Bank statements
+ Questionnaire forms

Web pages act like electronic versions of these documents.

### Why do you want your documents to have structure?

> __Structure__ is very important in helping readers to understand the messages you are trying to convey and to navigate around the document.

> __Structure__ helps readers understand the stories in the newspaper.

### What structure would you choose for your documents?

The one that allows you to communicate:
+ Hierarchy
+ Order

#### Tree structure

![](http://www.berndtgroup.net/~/media/images/thinking/blog/2014/deeptreestructure2.ashx)

+ [Article 1](trees/README.md)

### How do we describe a tree structure of a document to a web browser?

We use __HyperText Markup Language (HTML)__. It describes the (tree) structure of an HTML document.

1. __HyperText__ - refers to the fact that HTML allows you to create links that allow visitors to move from one page to another easily. _How would you navigate to another page without links?_

2. __Markup Language__ - allows you to annotate text, and these annotations provide additional meaning to the contents of a document.
  1. Structural markup - the elements that you can use to describe both headings and paragraphs.
  2. Semantic markup - the elements which provide extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation, etc.

__HTML document__ is made of __HTML elements__.

### What is an HTML element?

Example:

```html
<h1>Welcome to The Iron Yard.</h1>
```

Elements are usually made up of two __tags__:

1. An opening tag, e.g.: `<h1>`
2. A closing tag, e.g.: `</h1>`

__Opening tag__ is made of:

1. `<` - left-angle bracket (less-than sign).
2. `h1` - characters.
3. `>` - right-angle bracket (more-than sign).

__Closing tag__ is made of:

1. `<` - left-angle bracket (less-than sign).
2. `/` - forward slash.
3. `h1` - characters.
4. `>` - right-angle bracket (more-than sign).

> __Tags__ tell you something about the information that lies between thier opening and closing tags.

![](https://imgs.xkcd.com/comics/tags.png)

Here is a list of all tags in the latest version of HTML: https://developer.mozilla.org/en/docs/Web/HTML/Element

Tags can have __attributes__.

### What are tag attributes?

> Attributes provide additional information about the contents of an element. They appear on __the opening tag__ of the element and are made of two parts: a __name__ and a __value__, separated by an __equals__ sign.

Example:

```html
<a href="http://artemij.com"></a>
```

+ Attribute name: `href` - always in _lowercase_ - tell what kind of extra information you're supplying about the element's content.
+ Attribute value: `http://artemij.com` - tell extra information or setting for the attribute. __Important:__ always use __double quotes__.

Here is a list of all tag attributes in the latest version of HTML: https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes

### What is the structure of a valid HTML document?

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Welcome to The Iron Yard</title>
  </head>
  <body>
    <!-- Your information goes here... -->
  </body>
</html>
```

1. `<!DOCTYPE>` - informs the web browser which version of HTML you used to write the document. https://developer.mozilla.org/en-US/docs/Glossary/Doctype

2. The HTML `<html>` Element (or HTML root element) represents the root of an HTML document. All other elements must be descendants of this element. There can be only one `<html>` element in a document. https://developer.mozilla.org/en-US/docs/Web/HTML/Element/html

3. The HTML Head Element (`<head>`) provides general information (metadata) about the document, including its title and links to or definitions of scripts and style sheets. There can be only one `<head>` element in a document. https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head

3. The HTML Title Element (`<title>`) defines the title of the document, shown in a browser's title bar or on the page's tab. https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title

4. The HTML Body Element (`<body>`) represents the content of an HTML document. Everything inside of this element is rendered inside the browser window. There can be only one `<body>` element in a document. https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body

5. HTML comment begins with: `<!--`
6. HTML comment ends with: `-->`

### How to valide my HTML document?

Use W3C Markup Validator: https://validator.w3.org

### Why my whitespace is not displayed?

This:

```html
<p>This is the first week of      the full-time front   


            end




course.
</p>
```

will be rendered the same as this:

```html
<p>This is the first week of the full-time front end course.</p>
```

_Because_: when a web browser comes across two or more spaces next to each other, it only displays one spece.

It treats a line break as a single space too.

This is known as __white space collapsing__.

### Which HTML tag should I choose?

_A better question_: what is the semantics of the information enclosed inside of your HTML element?

![](http://imagesmtv-a.akamaihd.net/uri/mgid:file:http:shared:mtv.com/news/wp-content/uploads/2015/05/tumblr_m1icomdf8l1qfxq1qo1_500-1-1431394624.gif)

+ [Article 2](https://boagworld.com/dev/semantic-code-what-why-how/)
+ [Article 3](http://diveintohtml5.info/semantics.html)
+ [Article 4](http://learn.shayhowe.com/html-css/getting-to-know-html/)

### What if I have text?

#### Headings:

```html
<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>
```

+ [Example](http://jsbin.com/nufelagexo/edit?html,output)

#### Paragraphs

```html
<p></p>
```

+ [Example](http://jsbin.com/vekopimuka/edit?html,output)

#### Bold

```html
<b></b>
```

+ [Example](http://jsbin.com/difopimisu/edit?html,output)

### Italic

```html
<i></i>
```

+ [Example](http://jsbin.com/jokiwirigo/edit?html,output)

### Superscript

```html
<sup></sup>
```

+ [Example](http://jsbin.com/kigixocure/edit?html,output)

### Subscript

```html
<sub></sub>
```

+ [Example](http://jsbin.com/pujajecaqi/edit?html,output)

### Line breaks

```html
<br /> or <br>
```

+ [Example](http://jsbin.com/xesegojojo/edit?html,output)

### Horizontal rules

```html
<hr /> or <hr>
```

+ [Example](http://jsbin.com/hinodideja/edit?html,output)

> There are a few elements that do not have any words between an opening and closing tags. They are known as __empty elements__. Also known as __void elements__.

+ [Article 5](http://www.colorglare.com/2014/02/03/to-close-or-not-to-close.html)

## What if I have lists?

### Ordered list

Ordered lists use _numbers_.

```html
<ol>
  <li></li>
  <li></li>
  <li></li>
</ol>
```

`<li></li>` - list item.

### Unordered list

Unfordered lists use _bullets_.

```html
<ul>
  <li></li>
  <li></li>
  <li></li>
</ul>
```

### Definition list

Definition lists are used to define terminology.

```html
<dl>
  <dt></dt>
  <dd></dd>
  <dt></dt>
  <dd></dd>
  <dt></dt>
  <dd></dd>
</dl>
```

`<dt></dt>` - contains the definition term.
<br>
`<dd></dd>` - contains the definition.

### What if I have links?

```html
<a href="http://artemij.com">My website</a>
```

+ Absolute URL, e.g.: `http://artemij.com`
+ Relative URL, e.g.: `./index.html`

### Open links in a new window

```html
<a href="http://artemij.com" target="_blank">My website</a>
```

### Linking to a specific part of the same page

```html
<a href="#summary">Summary</a>
```

+ [Example](http://jsbin.com/lupozenoya/edit?html,output)

### Email link

```html
<a href="mailto:artemij.fedosejev@gmail.com">Email Art</a>
```

+ Mailto generator: http://www.mailto.co.uk

## What if I have images?

```html
<img src="http://artemij.com/images/react_essentials_book_cover.jpg" 
    alt="React.js Essentials book cover" 
    title="Written by Artemij Fedosejev"
    width="300" />
```

Result:

<img src="http://reactessentials.com/images/react-essentials-book-cover.jpg" 
    alt="React.js Essentials book cover" 
    title="Written by Artemij Fedosejev"
    width="300" />

__Required attributes:__
+ `src` attribute - tells the web browser where it can find the image file.
+ `alt` attribute - provides a text description of the image which describes the image if you cannot see it.

__Warning!__ Do not use `width` and `height` attributes to specify image size - _unless you absolutely have to_ - this should be done with CSS instead.

#### Have an image with captions?

Use `<figure>`:

```html
<figure>
  <img src="http://artemij.com/images/react_essentials_book_cover.jpg" 
    alt="React.js Essentials book cover" 
    title="Written by Artemij Fedosejev" />
  <br />
  <figcaption>
    Cover image of a book written by Artemij Fedosejev.
  </figcaption>
</figure>
```

+ [Example](http://jsbin.com/simusovugi/edit?html,output)

You can have more than one image inside of a figure as long as they all share the same caption.

#### What if I want to render a table?

Data examples: timetables, sport results, financial reports, etc.

```html
<table>
  <tr>
    <th>Tens</th>
    <th>Hundreds</th>
    <th>Thousands</th>
  </tr>
  <tr>
    <td>10</td>
    <td>20</td>
    <td>30</td>
  </tr>
  <tr>
    <td>100</td>
    <td>200</td>
    <td>300</td>
  </tr>
  <tr>
    <td>1000</td>
    <td>2000</td>
    <td>3000</td>
  </tr>
</table>
```

Result:

<table>
  <tr>
    <th>Tens</th>
    <th>Hundreds</th>
    <th>Thousands</th>
  </tr>
  <tr>
    <td>10</td>
    <td>20</td>
    <td>30</td>
  </tr>
  <tr>
    <td>100</td>
    <td>200</td>
    <td>300</td>
  </tr>
  <tr>
    <td>1000</td>
    <td>2000</td>
    <td>3000</td>
  </tr>
</table>

+ `<table></table>` - creates table.
+ `<th></th>` - creates heading for either column or row.
+ `<tr></tr>` - creates table row.
+ `<td></td>` - creates table data, i.e.: table cell.

Useful attributes:
+ `colspan`
+ `rowspan`

#### How can I create a form?

```html
<form action="http://artemij.com/login" method="post">
  <input type="text" name="username" />
  <input type="password" name="password" />
  <button>Login</button>
</form>
```

+ [Example](http://jsbin.com/kikapahoxa/edit?html,output)

How about other input types?

##### Radio button

```html
<form action="http://artemij.com/process" method="post">
  <input type="radio" name="genre" value="pop" selected="selected" /> Pop
  <input type="radio" name="genre" value="rock" /> Rock
  <input type="radio" name="genre" value="rap" /> Rap
  <button>Ok</button>
</form>
```

+ [Example](http://jsbin.com/mupokimobe/edit?html,output)

##### Checkbox

```html
<form action="http://artemij.com/process" method="post">
  <input type="checkbox" name="drink" value="water" /> Water
  <input type="checkbox" name="drink" value="tea" /> Tea
  <input type="checkbox" name="drink" value="coffee" /> Coffee
  <button>Ok</button>
</form>
```

+ [Example](http://jsbin.com/kofuloruki/edit?html,output)

##### What about labels?

```html
<form action="http://artemij.com/process" method="post">
  <input type="checkbox" name="drink" value="water" id="water" /> <label for="water">Water</label>
  <label><input type="checkbox" name="drink" value="tea" /> Tea</label>
  <label><input type="checkbox" name="drink" value="coffee" /> Coffee</label>
  <button>Ok</button>
</form>
```

+ [Example](http://jsbin.com/taqehupovu/edit?html,output)

##### Drop down list box

```html
<form action="http://artemij.com/process" method="post">
  <select name="phones">
    <option value="iphone6s">iPhone 6s</option>
    <option value="iphone6">iPhone 6</option>
    <option value="iphone5">iPhone 5</option>
  </select>
  <button>Ok</button>
</form>
```

+ [Example](http://jsbin.com/lehufomuna/edit?html,output)

##### Multiple select box

```html
<form action="http://artemij.com/process" method="post">
  <select name="flash" multiple="multiple" size="5">
    <option value="8gb">8GB</option>
    <option value="16gb">16GB</option>
    <option value="32gb">32GB</option>
    <option value="64gb">64GB</option>
    <option value="128gb">128GB</option>
    <option value="256gb">256GB</option>
  </select>
  <button>Ok</button>
</form>
```

+ [Example](http://jsbin.com/wiluvuweli/edit?html,output)

##### File input

```html
<form action="http://artemij.com/process" method="post">
  <input type="file" name="photo" />
  <br />
  <button>Upload</button>
</form>
```

+ [Example](http://jsbin.com/pulizifegu/edit?html,output)

##### Hidden input

```html
<form action="http://artemij.com/process" method="post">
  <input type="file" name="photo" />
  <input type="hidden" name="secret" value="not-for-user-to-see" />
  <br />
  <button>Upload</button>
</form>
```

+ [Example](http://jsbin.com/sedahozudo/edit?html,output)

## Examples of student portfolios

+ http://driiven.com/
+ http://ryanatkinson.tech/
+ http://rdanieldesign.com/richarddaniel/#/
+ http://kelleyrose.co/

## [Problems](problems.md)

![](http://i.imgur.com/4pvKx8O.gif)

+ [Problem 1](problems.md#problem-1)
+ [Problem 2](problems.md#problem-2)
+ [Problem 3](problems.md#problem-3)
+ [Problem 4](problems.md#problem-4)
+ [Problem 5](problems.md#problem-5)
+ [Problem 6](problems.md#problem-6)
+ [Problem 7](problems.md#problem-7)
+ [Problem 8](problems.md#problem-8)
+ [Problem 9](problems.md#problem-9)
+ [Problem 10](problems.md#problem-10)
+ [Problem 11](problems.md#problem-11)
+ [Problem 12](problems.md#problem-12)
+ [Problem 13](problems.md#problem-13)
+ [Problem 14](problems.md#problem-14)

## Learn more

1. HyperText Markup Language (HTML): https://en.wikipedia.org/wiki/HTML
2. List of all HTML tags: https://developer.mozilla.org/en/docs/Web/HTML/Element
3. List of all HTML tag attributes: https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes
4. Mozilla Developer Network (MDN): https://developer.mozilla.org
5. DOCTYPE: https://en.wikipedia.org/wiki/Document_type_declaration
6. W3C Markup Validator: https://validator.w3.org/
7. Semantic HTML: https://en.wikipedia.org/wiki/Semantic_HTML
8. Semantic code: What? Why? How?: https://boagworld.com/dev/semantic-code-what-why-how/
9. Semantics: http://diveintohtml5.info/semantics.html
10. Getting to know HTML: http://learn.shayhowe.com/html-css/getting-to-know-html/
11. To close or not to close: http://www.colorglare.com/2014/02/03/to-close-or-not-to-close.html
12. How to embed Google Maps: https://support.google.com/maps/answer/3544418?hl=en
