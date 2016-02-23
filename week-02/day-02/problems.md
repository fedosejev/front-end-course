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

## 2.

Given this HTML:

```html
<div class="container">
  <img src="http://reactessentials.com/images/react-essentials-book-cover.jpg" />
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc eget accumsan augue, id auctor dui. In nec ipsum elit. In eget odio congue, volutpat turpis semper, tempus ex. Mauris in gravida nisi, quis interdum libero. Aliquam vel molestie dolor. Donec tincidunt nec neque vitae convallis. Aenean a mi aliquam, auctor nisl posuere, faucibus urna. Nullam nunc lacus, blandit et mi id, interdum fermentum eros. Nullam eget porta lacus. Sed eleifend tellus nec malesuada mattis. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam consequat vitae purus tristique rhoncus. Ut luctus efficitur eros ut rhoncus.</p>
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
}

img {
  width: 150px;
  float: left;
}
```

Make sure the text doesn't overflow underneath the image.

## 3.

Refactor your portfolio to become responsive. Consider the following breakpoints:

1. __Phones__, less than `768px`.
2. __Tablets__, `768px` and up.
3. __Desktops__, `992px` and up.
4. __Large desktops__, `1200px` and up.