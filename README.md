<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Global Signal News</title>

<style>

body{
font-family: Arial;
margin:0;
background:#f5f5f5;
}

header{
background:black;
color:white;
padding:15px;
text-align:center;
}

nav{
background:red;
padding:10px;
text-align:center;
}

nav a{
color:white;
margin:10px;
text-decoration:none;
font-weight:bold;
}

.container{
padding:20px;
}

.news{
background:white;
padding:15px;
margin-bottom:20px;
border-radius:8px;
}

button{
background:red;
color:white;
border:none;
padding:8px 12px;
cursor:pointer;
}

footer{
background:black;
color:white;
text-align:center;
padding:10px;
}

</style>
</head>

<body>

<header>
<h1>Global Signal News</h1>
</header>

<nav>
<a href="#">Home</a>
<a href="#">World</a>
<a href="#">India</a>
<a href="#">Technology</a>
<a href="#">Sports</a>
</nav>

<div class="container">

<div class="news">
<h2>AI Technology Changing the World</h2>
<p>Artificial intelligence is transforming industries around the world with new tools and automation.</p>
<button onclick="speakNews('Artificial intelligence is transforming industries around the world.')">
🔊 Listen News
</button>
</div>

<div class="news">
<h2>Global Economy Update</h2>
<p>Experts predict new economic changes in global markets as technology grows rapidly.</p>
<button onclick="speakNews('Experts predict new economic changes in global markets.')">
🔊 Listen News
</button>
</div>

</div>

<footer>
<p>© 2026 Global Signal News</p>
</footer>

<script>

function speakNews(text){

let speech = new SpeechSynthesisUtterance(text);
speech.lang="en-US";

speechSynthesis.speak(speech);

}

</script>

</body>
</html>
