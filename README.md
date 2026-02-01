# Emilia-project-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Be My Valentine</title>
<style>
body {
  background: linear-gradient(to right, #ff758c, #ff7eb3);
  font-family: 'Arial', sans-serif;
  text-align: center;
  color: white;
  padding-top: 80px;
}
h1 { font-size: 2.5em; }
button {
  font-size: 1.2em;
  padding: 12px 25px;
  border: none;
  border-radius: 30px;
  margin: 15px;
  cursor: pointer;
}
#yes { background: #ff4d6d; color: white; }
#no { background: white; color: #ff4d6d; position: absolute; }
.hearts {
  position: fixed;
  top: 0; left: 0;
  width: 100%; height: 100%;
  pointer-events: none;
}
</style>
</head>

<body>
<h1>💘 EMILIA NDIDIAMAKA GILBERT 💘</h1>
<p>You make my world brighter, my days sweeter, and my heart softer.</p>
<h2>Will you be my Valentine? 🌹</h2>

<button id="yes" onclick="yes()">YES ❤️</button>
<button id="no" onmouseover="moveNo()">NO 💔</button>

<script>
function yes(){
  document.body.innerHTML =
  "<h1>❤️ She Said YES ❤️</h1><p>I can’t wait to make beautiful memories with you 🥰</p>";
}
function moveNo(){
  const btn = document.getElementById("no");
  btn.style.top = Math.random()*80 + "vh";
  btn.style.left = Math.random()*80 + "vw";
}
</script>
</body>
</html>