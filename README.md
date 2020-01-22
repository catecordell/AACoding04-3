<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<link rel="apple-touch-icon" type="image/png" href="https://static.codepen.io/assets/favicon/apple-touch-icon-5ae1a0698dcc2402e9712f7d01ed509a57814f994c660df9f7a952f3060705ee.png" />
<meta name="apple-mobile-web-app-title" content="CodePen">
<link rel="shortcut icon" type="image/x-icon" href="https://static.codepen.io/assets/favicon/favicon-aec34940fbc1a6e787974dcd360f2c6b63348d4b1f4e06c77743096d55480f33.ico" />
<link rel="mask-icon" type="" href="https://static.codepen.io/assets/favicon/logo-pin-8f3771b1072e3c38bd662872f6b673a722f4b3ca2421637d5596661b4e2132cc.svg" color="#111" />
<title>CodePen - AACoding04-2</title>
<style>
.correct{
  background:green;
}

.incorrect{
  background:red;
}
</style>
</head>
<body translate="no">
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<audio id="sad" controls>
<source src="https://math.seattleacademy.org/garyanderson/snd/sad.mp3" type="audio/mpeg">
</audio>
<div>Timer: <span id="theTimer">0</span> Score: <span id="score">0</span></div>
<h1>Cates Math Party</h1>
<ol>
<li> \( 2^3 \) <input data-correct="8" /> </li>
<li> \( \sqrt[3]{8} \) <input data-correct="2" /></li>
<li> \( 8^\frac{1}{3} \) <input data-correct="2" /></li>
<li> \( 27^\frac{-2}{3} \) <input data-correct="1/9" /></li>
<li> \( \sqrt[3]{27} \) <input data-correct="3" /> </li>
<li> \( 8^3 \) <input data-correct="512" /> </li>
<li> \( 8^\frac{2}{3} \) <input data-correct="4" /> </li>
<li> \( \sqrt[5]{243} \) <input data-correct="3" /> </li>
<li> \( 343^\frac{2}{3} \) <input data-correct="49" /> </li>
<li> \( 3^7 \) <input data-correct="2187" /> </li>
<ol>
<script src='https://cdnjs.cloudflare.com/ajax/libs/jquery/3.4.1/jquery.min.js'></script>
<script id="rendered-js">
const sad = document.getElementById("sad");
setInterval(onTimer, 1000);
function onTimer() {
  let theTimer = Number($("#theTimer").text());
  theTimer = theTimer + 1;
  $("#theTimer").text(theTimer);
}

$("input").change(onChange);

function onChange(evt) {
  let correct = $(this).data("correct");
  let response = $(this).val();
  if (correct == response) {
    let score = Number($("#score").text());
    score = score + 1;
    $("#score").text(score);
    $(this)
      .removeClass("incorrect")
      .addClass("correct");
  } else {
    $(this)
      .removeClass("correct")
      .addClass("incorrect");
    if (Math.random() > 0.9) {
      sad.play();
    }
  }
}
    </script>
</body>
</html>
