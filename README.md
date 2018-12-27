<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Fixed positioning</title>

    <style>
      body {
        width: 500px;
        height: 1400px;
        margin: 0 auto;
      }
      p {
        background: aqua;
        border: 3px solid blue;
        padding: 10px;
        margin: 10px;
      }
      span {
        background: red;
        border: 1px solid black;
      }
      h1 {
        position: fixed;
        top: 0px;
        width: 500px;
        margin: 0 auto;
        background: white;
        padding: 10px;
      }
      p:nth-of-type(1) {
        margin-top: 60px;
      }
    </style>
  </head>
  <body>
    <h1>Fixed positioning</h1>

    <p>I am a basic block level element. My adjacent block level elements sit on new lines below me.</p>

    <p class="positioned">Now I'm absolutely positioned relative to the <code>&lt;body&gt;</code> element, not the <code>&lt;html&gt;</code> element!</p>

    <p>We are separated by our margins. Because of margin collapsing, we are separated by the width of one of our margins, not both.</p>

    <p>inline elements <span>like this one</span> and <span>this one</span> sit on the same line as one another, and adjacent text nodes, if there is space on the same line. Overflowing inline elements <span>wrap onto a new line if possible — like this one containing text</span>, or just go on to a new line if not, much like this image will do: <img src="long.jpg"></p>

  </body>
</html>
