<html>
<head>
  <link rel="stylesheet" href="tabs.css">
  <h1>Sofware Projects</h1>
</head>
<script>
function openPage(evt, cityName) {
  // Declare all variables
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }

  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(cityName).style.display = "block";
  evt.currentTarget.className += " active";
} 
window.onload = function(){
var acc = document.getElementsByClassName("accordion");
var i;
for (i = 0; i < acc.length; i++) {
  acc[i].addEventListener("click", function() {
    this.classList.toggle("active");
    var panel = this.nextElementSibling;
    if (panel.style.display === "block") {
      panel.style.display = "none";
    } else {
      panel.style.display = "block";
    }
  });
}
document.getElementById("defaultOpen").click(); 
}
document.getElementsByClassName("tablinks")[1].className = "active";
</script>
<div class="btn-group">
  <button class="tablinks" onclick="openPage(event, '1')" id = "defaultOpen" >Java</button>
  <button class="tablinks" onclick="openPage(event, '2')">Python</button>
  <button class="tablinks" onclick="openPage(event, '3')">MATLAB</button>
  <button class="tablinks" onclick="openPage(event, '4')">C++</button>
  <button class="tablinks" onclick="openPage(event, '5')">C</button>
</div>

<div id="1" class="tabcontent">
  <h2>Java Projects</h2>
  <h3><a href =  "Software Projects/Patience">Patience (Solitaire)</a></h3>
  <p>Object Oriented playable game of Solitaire</p>
  <img src="Software Projects/Images/Patience.png"
     style="max-width: 100%;"/> 
  <h3>Backgammon</h3>
  <p>Object Oriented playable game of Backgammon. Created as part of a group assignment, using github for version control and JUnit testing for trouble shooting.</p>
  <img src="Software Projects/Images/Bg1.png"
     style="max-width: 100%;"/> 
  <img src="Software Projects/Images/Bg2.png"
     style="max-width: 100%;"/> 
</div>

<div id="2" class="tabcontent">
  <h2>Python Projects</h2>
  
</div>

<div id="3" class="tabcontent">
  <h2>MATLAB Projects</h2>
  
</div>

<div id="4" class="tabcontent">
  <h2>C++ Projects</h2>
  
</div>

<div id="5" class="tabcontent"></div>
  <h2>C Projects</h2>
  <h3><a href =  "Software Projects/C">Hangman</a></h3>
  <p>Playable game of Hangman, that uses txt file input as word and gives 10 work or letter guesses</p>
  <img src="Software Projects/Images/Hangman.png"
     style="max-width: 100%;"/> 
</html>
