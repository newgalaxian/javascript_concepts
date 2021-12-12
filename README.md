#  image rollover  (JavaScript basics concepts)

an image rollover to change the appearance of an image whenever a visitor
to the Web site moves the mouse pointer over the image.
![chrome-capture](https://user-images.githubusercontent.com/12398746/145710560-54dab01e-2db3-4c51-a5a7-dc0fb6ab5b56.gif)

    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>HTML and JavaScript</title>
       <script>
           var blueArrow = new Image;
           var redArrow = new Image;

         function startup() {
            blueArrow.src = "img/blueArrow.gif";
            redArrow.src = "img/redArrow.gif";
            return;
        }
        function turnBlue() {
            document.arrow.src = blueArrow.src;
            return;
        }
        function turnRed() {
            document.arrow.src = redArrow.src;
            return;
        }
       </script>
     </head>

        <body onLoad="startup()">
          <div align="center">
              <a href="js1.html" onmouseout="turnBlue()" onmouseover="turnRed()">
              <img name="arrow" src="img/blueArrow.gif"></a>
         </div>

        </body>

     </html>
