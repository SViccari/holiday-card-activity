# Step Two
---
# Add a Background Image
Every Christmas card needs a holiday image.

Rather than adding a background image for the entire webpage, we're going to add
 a background image to a `section` of the webpage.

In your `christmas_card.html` file, wrap the `<h1>` and `<h2>`
tags in a `section` tag.
Example:
```
<section>
  <h1>Your holiday greeting</h1>
  <h2>From: your name</h2>
</section>
```

Now that we've added the `section` tag, we can target this tag with css to add
our background image.

Open your `style.css` file. Add the following to your `style.css` file:
```
section {
  background: url(https://codecademy-content.s3.amazonaws.com/courses/web-beginner-en-9xjis/images/winter.jpg);
  width: 700px;
  height: 500px;
}
```

Notice that our background image is pulling an image from Codecademy. They are
the authors of this activity so we're using the image they have made
available for us.

Hmm... we successfully added a background image but now we can't see our greeting.
Let's fix that.

In your `style.css` file, make all text in the `section` tags white, like so:
```
section {
  background: url(https://codecademy-content.s3.amazonaws.com/courses/web-beginner-en-9xjis/images/winter.jpg);
  width: 700px;
  height: 500px;
  color: white;
}
```

To make our greeting more legible, let's increase the font size. In the same
`style.css` file, beneath the closing `}` for `section`, target the `<h1>`
and `<h2>` tags to set their font size.
```
h1 {
  font-size: 60px;
}

h2 {
  font-size: 30px;
}
```

# Position the Background Image
Did you notice how the amount of whitespace between the top of our picture and
the top of the web page increased? Why the heck did our image move down the page?
Our image moved down because the `<h1>` and `<h2>` tags automatically add
a top and bottom margin. If you open the browser inspect tool, and hover over
the `<h1>` tag, you'll see blocks of color above and below the `<h1>` tag that
represent the added margin. Let's fix this by setting the margin to zero.
Example:
```
h1 {
  margin: 0;
  font-size: 60px;
}

h2 {
  margin: 0;
  margin-top: 30px;
  font-size: 30px;
}
```
Notice that we added `margin-top: 30px` after resetting the margin to zero to
provide space between our two lines of text.
