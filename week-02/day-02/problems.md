# Problems

## 1.

Given this HTML:

```html
<div class="container">
  <p class="first">First</p>
  <p class="second">Second</p>
  <p class="third">Third</p>
</div>
```

And this CSS:

```css
@import url(https://fonts.googleapis.com/css?family=Roboto+Condensed);

* {
  margin: 0;
  padding: 0;
}

div {
  padding-top: 20px;
  padding-bottom: 20px;
  font-family: 'Roboto Condensed', sans-serif;
  text-align: center;
  text-transform: uppercase;
}

p {
  margin: 20px 0;
}

.first {
  background-color: rgb(95%, 90%, 45%);
}

.second {
  background-color: rgb(30%, 85%, 100%);
}

.third {
  background-color: rgb(10%, 95%, 90%);
}
```

Make sure all three paragraphs have margins that __do not collapse__.

## 1.

Refactor your portfolio to become responsive. Consider the following breakpoints:

1. __Phones__, less than `768px`.
2. __Tablets__, `768px` and up.
3. __Desktops__, `992px` and up.
4. __Large desktops__, `1200px` and up.