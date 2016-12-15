## Step Four

### Add Another Image
We have two images to choose from, you can add Santa or a Snowman. In your
`christmas_card.html` file, beneath the closing `</div>` tag for the `greeting`
class, add one of the following lines of code:

If you want Santa, add this line:
```
<img src="https://codecademy-content.s3.amazonaws.com/courses/web-beginner-en-9xjis/images/santa.png">
```
<img src="https://codecademy-content.s3.amazonaws.com/courses/web-beginner-en-9xjis/images/santa.png">

If you want a Snowman, add this line:
```
<img src="https://codecademy-content.s3.amazonaws.com/courses/web-beginner-en-9xjis/images/snowman.png">
```
<img src="https://codecademy-content.s3.amazonaws.com/courses/web-beginner-en-9xjis/images/snowman.png">

Your `christmas_card.html` file should look like this now:
```
<!DOCTYPE html>
<html>
  <head>
    <title>Happy Holidays!</title>
    <link rel="stylesheet" href="style.css" type="text/css">
  </head>
  <body>
  <section>
    <div class="greeting">
      <h1>Your holiday greeting</h1>
      <h2>From: your name</h2>
    </div>
    <img src="https://codecademy-content.s3.amazonaws.com/courses/web-beginner-en-9xjis/images/santa.png">
  </section>
  </body>
</html>
```

To move our image to a better location, we'll target the `img` tag. At the
bottom of your `style.css` file, add the following:
```
img {
  padding-top: 70px;
  padding-left: 140px;
}
```
Feel free to play around with the values to move your image to where you think
it looks best!
