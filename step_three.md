## Step Three

### Font
Is it just me, or is our font a bit boring? There are a number of free
fonts that Google makes available for us, we just need to import them into our
css file before we can use them.

In your `style.css` file, at the top of the file, add:
```
@import url(http://fonts.googleapis.com/css?family=Dancing+Script);
```

Now we can use the "Dancing Script" font by adding the following to `section`
in our css file:
```
section {
  background: url(https://codecademy-content.s3.amazonaws.com/courses/web-beginner-en-9xjis/images/winter.jpg);
  width: 700px;
  height: 500px;
  color: white;
  font-family: Dancing Script;
}
```

Interested in using a different font? Visit https://fonts.google.com to find
more fonts. Just remember to import the font you wish to use.

### Position Your Greeting
Let's move our greeting out of the corner so the text isn't flush with the
edge of the card. Before we add any css, let's wrap the greeting text in a css
class so we can easily apply css to the `<h1>` and `<h2>` tags at the same time.

In your `christmas_card.html` file, add a `greeting` class. Example:
```
<section>
  <div class="greeting">
    <h1>Your holiday greeting</h1>
    <h2>From: your name</h2>
  </div>
</section>
```
Now, let's style! In your `style.css` file, add the following:
```
.greeting {
  padding-top: 10px;
  padding-left: 20px;
}
```

**Pro-tip Detour**

If you like, you can shorten this to:
```
.greeting {
  padding: 10px 20px;
}
```
The reason we can shorten this is because the padding property can be
written using:
```
padding-bottom
padding-left
padding-right
padding-top
```
or, when provide two values to `padding`, this sets the vertical and horizontal
padding values (aka, `padding-left` and `padding-top`). Visit the [Mozilla
Developer Network](https://developer.mozilla.org/en-US/docs/Web/CSS/padding) for more details.

**End Detour**
