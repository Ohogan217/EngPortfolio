<html>
<head>
  <a href="https://ohogan217.github.io/">Return to Home</a> 
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
  <button class="tablinks" onclick="openPage(event, '3')" id = "defaultOpen">MATLAB</button>
  <button class="tablinks" onclick="openPage(event, '1')">Java</button>
  <button class="tablinks" onclick="openPage(event, '2')">Python</button>
  <button class="tablinks" onclick="openPage(event, '5')">C</button>
</div>

<div id="1" class="tabcontent">
  <h2>Java Projects</h2>
  <h3>Patience (Solitaire)</h3>
  <a href =  "https://github.com/Ohogan217/Ohogan217.github.io/tree/master/Software%20Projects/Java/Patience">Link to Project Files</a>
  <p>Object Oriented playable game of Solitaire</p>
  <img src="Software Projects/Images/Patience.png"
     style="max-width: 100%;"/> 
  <p></p>
  <h3>Backgammon</h3>
  <a href =  "https://github.com/Ohogan217/Group_34">Link to Project Files</a>
  
  
  <p>Object Oriented playable game of Backgammon. Created as part of a group assignment, using github for version control and JUnit testing for trouble shooting.</p>
  <img src="Software Projects/Images/Bg1.png"
     style="max-width: 100%;"/> 
  <img src="Software Projects/Images/Bg2.png"
     style="max-width: 100%;"/> 
</div>

<div id="2" class="tabcontent">
  <h2>Python Projects</h2>
  <h3>Myelinated Axon Simulation</h3>
  <a href =  "https://github.com/Ohogan217/Ohogan217.github.io/tree/master/Software%20Projects/Python">Link to Project Files</a>
  <p>Simulated the effect of various stimuli on myelinated axon firing rates, conductance velocity and membrane potential. Simulated using NEURON library and Jupyter Notebooks</p>
  <img src="Software Projects/Images/Axon.png"
     style="max-width: 100%;"/> 
</div>

<div id="3" class="tabcontent">
  <h2>MATLAB Projects</h2>
  <h3>Decision Making Trial Software</h3>
  <a href =  "https://github.com/Ohogan217/Ohogan217.github.io/tree/master/Software%20Projects/MATLAB/Thesis Software">Link to Project Files</a>
  
  <p>Object oriented decision making trial package that could utilise a discrete user input using two force sensors. This uses MATLAB with the PsychToolbox package and a National Instruments DAQ to read in the real time force values</p>
  <img src="Software Projects/Images/DMTrial.png"
     style="max-width: 100%;"/> 
     <p></p>
  <h3>Machine Learning Parkinson's Diagnosis</h3>
  <a href =  "https://github.com/Ohogan217/Ohogan217.github.io/tree/master/Software%20Projects/Matlab/Machine%20Learning">Link to Project Files</a>
  <p>Comparison of machine learning algorithms to assess suitability to diagnose parkinson's based on pressure sensor walking data</p>
  <p></p>
  <h3>Bridge Stress Simulation</h3>
  <a href =  "https://github.com/Ohogan217/Ohogan217.github.io/tree/master/Software%20Projects/Matlab/Modelling and Simulation">Link to Project Files</a>
  <p>3D modelled truck driving over a truss bridge, with colours of the beams that demonstrate the relative compression or tension within it. This simulation was carried out in MATLAB.</p>
  <img src="Software Projects/Images/MnS.gif"
     style="max-width: 100%;"/> 
</div>

<div id="4" class="tabcontent">
  <h2>C++ Projects</h2>
  
</div>

<div id="5" class="tabcontent">
  <h2>C Projects</h2>
  <h3>Hangman</h3>
  <a href =  "https://github.com/Ohogan217/Ohogan217.github.io/tree/master/Software%20Projects/C">Link to Project Files</a>
  <p>Playable game of Hangman, that uses txt file input as word and gives 10 work or letter guesses</p>
  <img src="Software Projects/Images/Hangman.png"
     style="max-width: 100%;"/> 
</div>
</html>
