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
  <button class="tablinks" onclick="openPage(event, '3')">Matlab</button>
  <button class="tablinks" onclick="openPage(event, '4')">C++</button>
  <button class="tablinks" onclick="openPage(event, '5')">C</button>
</div>

<div id="1" class="tabcontent"></div>

<div id="2" class="tabcontent"></div>

<div id="3" class="tabcontent"></div>

<div id="4" class="tabcontent"></div>

<div id="5" class="tabcontent"></div>

</html>
