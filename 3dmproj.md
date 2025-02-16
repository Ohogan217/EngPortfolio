<html>
<head>
   <link rel="stylesheet" href="tabs.css">
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
</script>

<div class="btn-group">
  <button class="tablinks" onclick="openPage(event, '1')">Popliteal Stent</button>
  <button class="tablinks" onclick="openCity(event, '2')">Electrodeposition<br>System</button>
  <button class="tablinks" onclick="openCity(event, '3')">Guitar Strummer</button>
  <button class="tablinks" onclick="openCity(event, '4')">Mars Rover<br>Wheel</button>
   
</div>

<div id="1" class="tabcontent">
  <h2>Popliteal Stent</h2>
  <p>Model and simulate stresses in in the popliteal artery after stent has been applied.</p>
  <p>Model stresses in the stent during expansion and after expansion for 2 different materials</p>
  <h3>Artery Simulation</h3>
  <img src="3d Modelling Projects/Popliteal Stent/UnstentedArtery.png"
     style="max-width: 70%;"/> 
  <img src="3d Modelling Projects/Popliteal Stent/StentedArtery.png" 
     style="max-width: 70%;"/> 
  <img src="3d Modelling Projects/Popliteal Stent/ArteryStress.png" 
     style="max-width: 70%;"/> 
 <h3>Stent Modelling</h3>
 <p>Stent was designed by creating a single cell that was duplicated 4 times to produce the desired shape. This was because the student version of Abaqus has a limit on the amount of Ngons for Finite Element Analysis.</p>
  <img src="3d Modelling Projects/Popliteal Stent/UnexpandedStent.png" 
     style="max-width: 70%;"/> 
  <img src="3d Modelling Projects/Popliteal Stent/StentUnitDesign.png" 
     style="max-width: 70%;"/> 
  <h3>Material Modelling</h3>
  <h4>Steel Stent</h4>
  <img src="3d Modelling Projects/Popliteal Stent/ExpansionStentSteel.png" 
     style="max-width: 70%;"/> 
  <img src="3d Modelling Projects/Popliteal Stent/ExpandedStentSteel.png" 
     style="max-width: 70%;"/> 
  <h4>Nitinol Stent</h4>
  <img src="3d Modelling Projects/Popliteal Stent/ExpansionStentNitinol.png" 
     style="max-width: 70%;"/> 
  <img src="3d Modelling Projects/Popliteal Stent/ExpandedStentNitinol.png" 
     style="max-width: 70%;"/> 
  <h4>Stent Stress Comparison</h4>
  <img src="3d Modelling Projects/Popliteal Stent/MatStressCompGraph.png" 
     style="max-width: 70%;"/> 
  
 
</div>

<div id="2" class="tabcontent">
  <h2>Electrodeposition System</h2>
  <p>Design an electrodeposition system for use on silicon chips</p>
 <img src="3d Modelling Projects/Electrodeposition System/FullSystem.png" 
     style="max-width: 70%;"/>
 <p></p>
 
 
<button class="accordion" >Renderings</button>
<div class="panel">
  <h2>Renderings</h2>
  <h3>Rotating Cathode Holder</h3>
  <img src="3d Modelling Projects/Electrodeposition System/Cathode render.png"  
     style="max-width: 70%;"/>
  <img src="3d Modelling Projects/Electrodeposition System/Cathode open.png" 
     style="max-width: 70%;"/> 

  <h3>Anode Basket</h3>
  <img src="3d Modelling Projects/Electrodeposition System/Anode Render.png" 
     style="max-width: 70%;"/>
</div>

<button class="accordion" >Drawings</button>
<div class="panel">
      <h2>Drawings</h2>
      <img src="3d Modelling Projects/Electrodeposition System/CathodeAssembly.png" 
     style="max-width: 70%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/TopDraw.png" 
     style="max-width: 70%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/ClaspDraw.png" 
     style="max-width: 70%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/PinDraw.png" 
     style="max-width: 70%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/RingDraw.png" 
     style="max-width: 70%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/FoamDraw.png" 
     style="max-width: 70%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/CaseDraw.png" 
     style="max-width: 70%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/ShaftDraw.png" 
     style="max-width: 70%;"/>
 </div>
</div>
<div id="3" class="tabcontent">
  <h2>Guitar Strummer</h2>
  <p>Develop a four bar linkage system for a specific purpose. A guitar strummer was chosen.</p>
  <img src="3d Modelling Projects/Guitar Strummer/MS.gif" 
     style="max-width: 70%;"/>

</div>

<div id="4" class="tabcontent">
  <h2>Mars Rover Wheel</h2>
  <p>Who we are and what we do.</p>
</div> 


