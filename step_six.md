# Step Six
---
# Add Snow

Codecademy has already written javascript code that will produce snow for us. (Thanks codecademy!) We just have to include their code in our html file.

In your `christmas_card.html` file, copy and paste the following between the `<head>` tags.
```
<script src="http://cdnjs.cloudflare.com/ajax/libs/jquery/1.8.3/jquery.min.js"></script>
<script src="http://s3.amazonaws.com/codecademy-content/courses/holiday-cards/snowfall.min.js"></script>
<script>
$(document).ready(function() {
    snowFall.snow($("section"), {
        minSize: 1,
        maxSize: 5,
        round: true,
        minSpeed: 1,
        maxSpeed: 3,
        flakeCount: 120
    });
});
</script>
```

Your `christmas_card.html` file should look like this now:
```
<!DOCTYPE html>
<html>
  <head>
    <title>Happy Holidays!</title>
    <link rel="stylesheet" href="style.css" type="text/css">
    <script src="http://cdnjs.cloudflare.com/ajax/libs/jquery/1.8.3/jquery.min.js"></script>
    <script src="http://s3.amazonaws.com/codecademy-content/courses/holiday-cards/snowfall.min.js"></script>
    <script>
      $(document).ready(function() {
        snowFall.snow($("section"), {
          minSize: 1,
          maxSize: 5,
          round: true,
          minSpeed: 1,
          maxSpeed: 3,
          flakeCount: 120,
        });
      });
    </script>
  </head>
  <body>
    <section>
      <h1>Your holiday greeting here</h1>
      <h2>From: <your name></h2>
      <img src="https://codecademy-content.s3.amazonaws.com/courses/web-beginner-en-9xjis/images/santa.png">
    </section>
  </body>
</html>
```

Have fun and play with the `flakeCount` to create a blizzard!
