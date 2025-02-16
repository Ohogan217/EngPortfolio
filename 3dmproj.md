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


<button class="tablink" onclick="openPage('1', this, 'red')" id="defaultOpen">Popliteal Stent</button>
<button class="tablink" onclick="openPage('2', this, 'green')">Electrodeposition System</button>
<button class="tablink" onclick="openPage('3', this, 'blue')">Guitar Strummer</button>
<button class="tablink" onclick="openPage('4', this, 'orange')">Mars Rover Wheel</button>
<button class="tablink" onclick="openPage('5', this, 'orange')">Toy Boat</button>

<div id="1" class="tabcontent">
  <h2>Popliteal Stent</h2>
  <p>Model and simulate stresses in in the popliteal artery after stent has been applied.</p>
  <p>Model stresses in the stent during expansion and after expansion for 2 different materials</p>
  <h3>Artery Simulation</h3>
  <img src="3d Modelling Projects/Popliteal Stent/UnstentedArtery.png"/>
  <img src="3d Modelling Projects/Popliteal Stent/StentedArtery.png"/>
  <img src="3d Modelling Projects/Popliteal Stent/ArteryStress.png"/>
 <h3>Stent Modelling</h3>
 <p>Stent was designed by creating a single cell that was duplicated 4 times to produce the desired shape. This was because the student version of Abaqus has a limit on the amount of Ngons for Finite Element Analysis.</p>
  <img src="3d Modelling Projects/Popliteal Stent/UnexpandedStent.png"/>
  <img src="3d Modelling Projects/Popliteal Stent/StentUnitDesign.png"/>
  <h3>Material Modelling</h3>
  <h4>Steel Stent</h4>
  <img src="3d Modelling Projects/Popliteal Stent/ExpansionStentSteel.png"/>
  <img src="3d Modelling Projects/Popliteal Stent/ExpandedStentSteel.png"/>
  <h4>Nitinol Stent</h4>
  <img src="3d Modelling Projects/Popliteal Stent/ExpansionStentNitinol.png"/>
  <img src="3d Modelling Projects/Popliteal Stent/ExpandedStentNitinol.png"/>
  <h4>Stent Stress Comparison</h4>
  <img src="3d Modelling Projects/Popliteal Stent/MatStressCompGraph.png"/>
  
 
</div>

<div id="2" class="tabcontent">
  <h2>Electrodeposition System</h2>
  <p>Design an electrodeposition system for use on silicon chips</p>
  <h3>Rotating Cathode Holder</h3>
  <img src="3d Modelling Projects/Electrodeposition System/Cathode render.png"/>
  <img src="3d Modelling Projects/Electrodeposition System/Cathode open"/> 
  <h3>Anode Basket</h3>
  <img src="3d Modelling Projects/Electrodeposition System/Anode render"/>
  <h3>Full System</h3>
  <img src="3d Modelling Projects/Electrodeposition System/Cathode render.png"/>
  <img src="3d Modelling Projects/Electrodeposition System/Cathode open"/> 
</div>

<div id="3" class="tabcontent">
  <h2>Guitar Strummer</h2>
  <p>Get in touch, or swing by for a cup of coffee.</p>
</div>

<div id="4" class="tabcontent">
  <h2>Mars Rover Wheel</h2>
  <p>Who we are and what we do.</p>
</div> 

<div id="5" class="tabcontent">
  <h2>Toy Boat</h2>
  <p>Who we are and what we do.</p>
</div> 
</html>
