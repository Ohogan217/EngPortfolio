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
  function openCity(evt, cityName) {
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
</script>


<button class="tablink" onclick="openPage('1', this, '#8EBFE3')" id="defaultOpen">Popliteal Stent</button>
<button class="tablink" onclick="openPage('2', this, '#8EBFE3')">Electrodeposition System</button>
<button class="tablink" onclick="openPage('3', this, '#8EBFE3')">Guitar Strummer</button>
<button class="tablink" onclick="openPage('4', this, '#8EBFE3')">Mars Rover Wheel</button>
<button class="tablink" onclick="openPage('5', this, '#8EBFE3')">Toy Boat</button>

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
  <!-- Tab links -->
<div class="tab">
  <button class="tablinks" onclick="openCity(event, 'London')">London</button>
  <button class="tablinks" onclick="openCity(event, 'Paris')">Paris</button>
  <button class="tablinks" onclick="openCity(event, 'Tokyo')">Tokyo</button>
</div>

<!-- Tab content -->
<div id="London" class="tabcontent">
  <h3>London</h3>
  <p>London is the capital city of England.</p>
</div>

<div id="Paris" class="tabcontent">
  <h3>Paris</h3>
  <p>Paris is the capital of France.</p>
</div>

<div id="Tokyo" class="tabcontent">
  <h3>Tokyo</h3>
  <p>Tokyo is the capital of Japan.</p>
</div> 
  
 
  <h2>Renders</h2>
  <h3>Rotating Cathode Holder</h3>
  <img src="3d Modelling Projects/Electrodeposition System/Cathode render.png"  
     style="max-width: 70%;"/>
  <img src="3d Modelling Projects/Electrodeposition System/Cathode open.png" 
     style="max-width: 70%;"/> 

  <h3>Anode Basket</h3>
  <img src="3d Modelling Projects/Electrodeposition System/Anode Render.png" 
     style="max-width: 70%;"/>
  </div>
  
  <h2>Drawings</h2>
 </div>
  
  
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
