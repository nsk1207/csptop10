 <html>
  <head>
    <title>Top 10 Video Games of the Year</title>
  </head>
  <body>
    <h1>Top 10 Video Games of the Year</h1>
    <form>
      <label>Which video game do you think was the best this year?</label><br>
      <input type="radio" name="vote" value="1) "> Stray (PC and Playstation)<br>
      <input type="radio" name="vote" value="2) "> Splatoon 3 (Nintendo Switch)<br>
      <input type="radio" name="vote" value="3) "> Neon White (PC and Nintendo Switch)<br>
      <input type="radio" name="vote" value="4) "> Elden Ring (PC, Playstation and Xbox)<br>
      <input type="radio" name="vote" value="5) "> Pokemon Legends: Arceus (Nintendo Switch)<br>
      <input type="radio" name="vote" value="6) "> God of War Ragnarok (Playstation)<br>
      <input type="radio" name="vote" value="7) "> Kirby and the Forgotten Land (Nintendo Switch)<br>
      <input type="radio" name="vote" value="8) "> Call of Duty Modern Warfare (PC, Xbox and Playstation)<br>
      <input type="radio" name="vote" value="9) "> OlliOlli World (PC, Xbox, Playstation and Nintendo Switch)<br>
      <input type="radio" name="vote" value="10) "> XenoBlade Chronicles 3 (Nintendo Switch)<br>
      <input type="submit" value="Vote">
    </form>

<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.collapsible {
  background-color: #777;
  color: white;
  cursor: pointer;
  padding: 20px;
  width: 100%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
}

</style>
</head>
<body>

<button type="button" class="collapsible">Not familiar with any of these games? Click here to read a brief description of each one!</button>
<div class="content">
  <p>Blah Blah Blah</p>
</div>

<script>
var coll = document.getElementsByClassName("collapsible");
var i;

for (i = 0; i < coll.length; i++) {
  coll[i].addEventListener("click", function() {
    this.classList.toggle("active");
    var content = this.nextElementSibling;
    if (content.style.display === "block") {
      content.style.display = "none";
    } else {
      content.style.display = "block";
    }
  });
}
</script>

</body>
    <br>
    <h2>Current Vote Counts = </h2>
    <div id="vote-counts">
      <!-- Vote counts will be displayed here -->
    </div>
  </body>
</html>




 

