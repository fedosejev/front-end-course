# Width, maximum width and box-sizing

## Box-sizing

Notice the following CSS selector:

```css
.box {
  box-sizing: border-box;
  width: 350px;
  padding: 20px;
  margin: 20px;
  color: white;
  background-color: royalblue;
}
```

Inspect that element in Chrome, then remove `box-sizing: border-box;` and inspect it again.

Noticed the difference?

## Width and max-width

Note the following CSS selectors:

```css
p {
  width: 60%;
  background-color: rgb(220, 220, 220);
  text-align: center;
}

.centered {
  margin: 0 auto;
  max-width: 500px;
}
```

As a result, this element's width is 60% of it's parent container, but the maximum width is 500px:

```html
<p class="centered">...</p>
```