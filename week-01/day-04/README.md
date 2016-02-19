# Day 4

![](http://media.giphy.com/media/KVtlLhFsWFQaI/giphy.gif)

Questions:

1. [How to style an HTML document?](#how-to-style-an-html-document)
2. [How to include CSS rules within an HTML page?](#how-to-include-css-rules-within-an-html-page)
3. [How to link an external CSS file?](#how-to-link-an-external-css-file)
4. [What selectors can I use?](#what-selectors-can-i-use)
5. [How to change colour?](#how-to-change-colour)
6. [How to change font?](#how-to-change-font)
7. [How to use external font?](#how-to-use-external-font)
8. [How to style font?](#how-to-style-font)
9. [How to style list?](#how-to-style-list)
10. [How to style table?](#how-to-style-table)
11. [What is specificity?](#what-is-specificity)
12. [What is box model?](#what-is-box-model)
13. [How to change element's position?](#how-to-change-elements-position)

Plus:

+ [Problems](problems.md)
+ [Learn more](#learn-more)

## Questions

### How to style an HTML document?

Example:

```css
p {
  font-size: 20px;
}
```

+ `p` - selector.
+ `{ font-size: 20px; }` - declation block.
+ `font-size: 20px` - declaration.
+ `font-size` - property.
+ `20px` - value.

### How to include CSS rules within an HTML page?

Place them inside of `<style></style>` tag that is inside of `<head></head>` tag.

+ __Advantages__: HTML and CSS code in one file.
+ __Disadvantages__: Can't reuse if you have more pages that have the same (similar) styling.

### How to link an external CSS file?

External style sheet file:

```html
<link href="styles.css" type="text/css" rel="stylesheet" />
```

+ __Advantages__: Can reuse if you have more than pages that have the same (similar) styling.
+ __Disadvantages__: Need to load external file (at least once per entire website).

### What selectors can I use?

<table>

  <tr>
    <th>
      Selectors
    </th>
    <th>
      Meaning
    </th>
  </tr>

  <tr>
    <th>
      Universal selector
    </th>
    <td>
      Applies to all elements in the document.
      <br/>
      Example:
      <br/>
      <code>* {}</code>
    </td>
  </tr>

  <tr>
    <th>
      Type selector
    </th>
    <td>
      Matches element names.
      <br/>
      Example:
      <br/>
      <code>h1, h2, h3 {}</code>
    </td>
  </tr>

  <tr>
    <th>
      Class selector
    </th>
    <td>
      Matches an element whose <class>class</class> attribute has a value that matches the one specificied after the full stop symbol.
      <br/>
      Example:
      <br/>
      <code>.primary {}</code>
    </td>
  </tr>

  <tr>
    <th>
      Pseudo-class selector
    </th>
    <td>
      Matches an element whose <class>state</class> matches the one specificied after the colon.
      <br/>
      Example:
      <br/>
      <code>:focus</code>
    </td>
  </tr>

  <tr>
    <th>
      Attribute selector
    </th>
    <td>
      Matches elements that have <class>attribute</class> name.
      <br/>
      Example:
      <br/>
      <code>[data-information="country"]</code>
    </td>
  </tr>

  <tr>
    <th>
      Id selector
    </th>
    <td>
      Matches an element whose <class>id</class> attribute has a value that matches the one specificied after the hash symbol.
      <br/>
      Example:
      <br/>
      <code>#introduction {}</code>
    </td>
  </tr>

  <tr>
    <th>
      Child selector
    </th>
    <td>
      Matches an element that is a direct child of anohter.
      <br/>
      Example:
      <br/>
      <code>li > a {}</code>
    </td>
  </tr>

  <tr>
    <th>
      Descendant selector
    </th>
    <td>
      Matches an element that is a descendent of another specified element (not just a direct child of that element).
      <br/>
      Example:
      <br/>
      <code>p a {}</code>
    </td>
  </tr>

  <tr>
    <th>
      Adjacent sibling selector
    </th>
    <td>
      Matches an element that is the next sibling of another.
      <br/>
      Example:
      <br/>
      <code>h1 + p {}</code>
    </td>
  </tr>

  <tr>
    <th>
      General sibling selector
    </th>
    <td>
      Matches an element that is a sibling of another, although it does not have to be the directly preceding element.
      <br/>
      Example:
      <br/>
      <code>h1 ~ p {}</code>
      <br/>
      Explanation: http://stackoverflow.com/a/10782297
    </td>
  </tr>

</table>

+ Explore more selecters: __[Article 1](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference#Selectors)__

### How to change colour?

__Group exercise:__

__2__ people in a group.<br />
__15__ minutes maximum.

1. Group 1: research and explain __HEX__ colour value.
2. Group 2: research and explain __RGB__ colour value.
3. Group 3: research and explain __RGBA__ colour value.
4. Group 4: research and explain __HLS__ colour value.

#### Foreground colour

```css

/* Colour name */
h1 {
  color: blue;
}

/* Colour HEX value */
h2 {
  color: #0000ff;
}

/* Short version of colour HEX value */
h2 {
  color: #00f;
}

/* RGB value (Red Green Blue) */
h3 {
  color: rgb(0, 0, 255);
}

/* RGBA value (Red Green Blue Aplha) */
h4 {
  color: rgba(0, 0, 255, 0.5);
}
```

+ __Colour names__: there are __147__ predefined colour names that are recognised by web browsers.
+ __HEX codes__: these are dix-digit codes that represent the amount of red, green and blue in a color, preceded by a hash sign.
+ __RGB values__: these express colors in terms of how much red, green, and blue are used to make it up.
+ __RGBA values__: same as RGB but with extra Alpha value - a number between `0.0` and `1.0`
  + `0.0` - 0% visible.
  + `1.0` - 100% visible.

Values for various colous: http://colours.neilorangepeel.com/

Try for yourself in [JSBin](http://jsbin.com)!

+ __[Article 2](http://www.smashingmagazine.com/2012/10/the-code-side-of-color/)__

#### Background colour

```css
h1 {
  background-color: #000;
}
```

Can use colour name, HEX value, RGB value, etc.

_Ensure that there is enough contrast between foreground and background colours._

### How to change font?

#### Typeface

+ Serif
+ Sans-serif
+ Monospace

#### Font family

```css
p {
  font-family: Arial, Verdana, sans-serif;
}

h1, h2, h3, h4, h5, h6 {
  font-family: "Courier New", Courier, monospace;
}
```

Usually you expect at least one of these fonts installed on user's computer.

### How to use external font?

```css
@import url(https://fonts.googleapis.com/css?family=Slabo+27px);

p {
  font-family: 'Slabo 27px', serif;
}
```

+ `@import` allows to import style rules from other style sheets.

### How to style font?

+ `font-weight` - allows you to create bold text.
+ `font-style` - allows you to create italic text.
+ `text-transformation` - allows you to change the case:
  + to `uppercase`
  + to `lowercase`
  + to `capitalize`
+ `text-decoration` - allows you to underline, overline, line-though your text.

### How to style list?

#### `list-style-type`

```css
ol {
  list-style-type: lower-roman;
}

ul {
  list-style-type: none;
}
```

#### `list-style-image`

```css
ul {
  list-style-image: url("images/star.png");
}
```

#### `list-style-position`

```css
ul {
  list-style-position: inside;
}
```

+ What's the shorthand property?

### How to style table?

Use:
+ `border-top`
+ `border-right`
+ `border-bottom`
+ `border-left`
+ `width`
+ `empty-cells`
+ `border-spacing`
+ `border-collapse`

### What is specificity?

CSS selectors can be more specific or less specific. More specific selectors win.

#### How to calculate specificity?

<table>
  <tr>
    <th>Points</th>
    <th>Selector type</th>
  </tr>
  <tr>
    <td>10000</td>
    <td>
      !important
      <br/>
      <code>color: red !important;</code>
    </td>
  </tr>
  <tr>
    <td>1000</td>
    <td>
      Inline style attribute
      <br/>
      <code>style="color: red;"</code>
    </td>
  </tr>
  <tr>
    <td>100</td>
    <td>
      Id
      <br/>
      <code>#important</code>
    </td>
  </tr>
  <tr>
    <td>10</td>
    <td>
      <table>
        <tr>
          <th>Class</th>
          <th>Pseudo-class</th>
          <th>Attribute</th>
          <th>Attribute</th>
        </tr>
        <tr>
          <td><code>.success</code></td>
          <td><code>:hover</code></td>
          <td><code>[data-message]</code></td>
          <td><code>[data-message="welcome"]</code></td>
        </tr>
      </table>
    </td>
  </tr>
  <tr>
    <td>1</td>
    <td>
      Element
      <br />
      <code>p</code>
    </td>
  </tr>
</table>

Examples:

+ `p#important .success` = 111 points.
+ `body p` = 2 points.
+ `body .success div` = 12 points.

In more details:

+ [Article 3](https://css-tricks.com/specifics-on-css-specificity/)

### What is box model?

The basis of CSS layout.

![](https://mdn.mozillademos.org/files/8685/boxmodel-(3).png)

+ [Example](http://jsbin.com/meripepaha/edit?html,css,output)

#### `box-sizing`

```css
h1 {
  background-color: #eee;

  width: 200px;
  border: 5px solid red;
  padding: 20px;
  margin: 20px;

  box-sizing: border-box;
}
```

+ [Example](http://jsbin.com/lohazavoli/edit?html,css,output)

### How to change element's position?

+ Use `position` property.
+ Use `top`, `left`, `bottom`, `right` properties.

+ [Example](http://jsbin.com/zuzozebena/edit?html,css,output)

## [Problems](problems.md)

+ [Problem 1](problems.md#problem-1)
+ [Problem 2](problems.md#problem-2)
+ [Problem 3](problems.md#problem-3)
+ [Problem 4](problems.md#problem-4)
+ [Problem 5](problems.md#problem-5)
+ [Problem 6](problems.md#problem-6)

## Learn more

1. The Code Side Of Color: http://www.smashingmagazine.com/2012/10/the-code-side-of-color/
2. Colours: http://colours.neilorangepeel.com/
3. Color Hex Color Codes: http://www.color-hex.com/
4. Google Fonts: https://www.google.com/fonts
5. Example of Google Fonts: http://jsbin.com/paxupu/edit?html,output
6. CSS Font Sizing: http://bitsofco.de/2015/css-font-sizing/?utm_source=designernews
7. Specifics on CSS Specificity: https://css-tricks.com/specifics-on-css-specificity/
8. Specificity calculator: http://specificity.keegan.st/
9. CSS validator: http://jigsaw.w3.org/css-validator/
10. Top margin and inline element: http://stackoverflow.com/a/10324608
11. A to Z CSS: http://www.atozcss.com/
12. Google HTML/CSS Style Guide: https://google.github.io/styleguide/htmlcssguide.xml
13. http://tympanus.net/codrops/css_reference/
14. http://jsbin.com/pebayafoha/edit?html,css,output
15. http://www.colorhexa.com/
