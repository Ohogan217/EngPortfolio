<html>
<style>
 link rel="stylesheet" href="tabs.css">
</style>
<script>
function openPage(pageName, elmnt, color) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].style.backgroundColor = "";
  }
  document.getElementById(pageName).style.display = "block";

  elmnt.style.backgroundColor = color;
  }
  window.onload = function() {
    
    document.getElementById("defaultOpen").click();
  };
</script>


<button class="tablink" onclick="openPage('1', this, 'red')" id="defaultOpen">Home</button>
<button class="tablink" onclick="openPage('2', this, 'green')">News</button>
<button class="tablink" onclick="openPage('3', this, 'blue')">Contact</button>
<button class="tablink" onclick="openPage('4', this, 'orange')">About</button>

<div id="1" class="tabcontent">
  <h3>Home</h3>
  <p>Home is where the heart is..</p>
</div>

<div id="2" class="tabcontent">
  <h3>News</h3>
  <p>Some news this fine day!</p>
</div>

<div id="3" class="tabcontent">
  <h3>Contact</h3>
  <p>Get in touch, or swing by for a cup of coffee.</p>
</div>

<div id="4" class="tabcontent">
  <h3>About</h3>
  <p>Who we are and what we do.</p>
</div> 
</html>
