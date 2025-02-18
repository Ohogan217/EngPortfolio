<html>
<head>
   <link rel="stylesheet" href="tabs.css">
<a href="https://ohogan217.github.io/">Return to Home</a> 
   
<h1>3D Modelling Projects</h1>
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

document.getElementsByClassName("tablinks")[1].className = "active";

let slideIndex = 2;
showSlides(slideIndex);
}
// Next/previous controls
function plusSlides(n) {
  showSlides(slideIndex += n);
}

// Thumbnail image controls
function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className = " active";
} 

</script>

<div class="btn-group">
  <button class="tablinks" onclick="openPage(event, '1')" id = "defaultOpen" >Popliteal<br>Stent</button>
  <button class="tablinks" onclick="openPage(event, '2')">Electrodeposition<br>System</button>
  <button class="tablinks" onclick="openPage(event, '3')">Guitar<br>Strummer</button>
  <button class="tablinks" onclick="openPage(event, '4')">Mars Rover<br>Wheel</button>
  <button class="tablinks" onclick="openPage(event, '5')">Misecellaneous<br>Renders</button>
  
   
</div>

<div id="1" class="tabcontent">
  <h2>Popliteal Stent</h2>
  <p>Model and simulate stresses in in the popliteal artery after stent has been applied.</p>
  <p>Model stresses in the stent during expansion and after expansion for 2 different materials</p>
  <h3>Artery Simulation</h3>
  <img src="3d Modelling Projects/Popliteal Stent/UnstentedArtery.png"
     style="max-width: 100%;"/> 
  <img src="3d Modelling Projects/Popliteal Stent/StentedArtery.png" 
     style="max-width: 100%;"/> 
  <img src="3d Modelling Projects/Popliteal Stent/ArteryStress.png" 
     style="max-width: 100%;"/> 
 <h3>Stent Modelling</h3>
 <p>Stent was designed by creating a single cell that was duplicated 4 times to produce the desired shape. This was because the student version of Abaqus has a limit on the amount of Ngons for Finite Element Analysis.</p>
  <img src="3d Modelling Projects/Popliteal Stent/UnexpandedStent.png" 
     style="max-width: 100%;"/> 
  <img src="3d Modelling Projects/Popliteal Stent/StentUnitDesign.png" 
     style="max-width: 100%;"/> 
  <h3>Material Modelling</h3>
  <h4>Steel Stent</h4>
  <img src="3d Modelling Projects/Popliteal Stent/ExpansionStentSteel.png" 
     style="max-width: 100%;"/> 
  <img src="3d Modelling Projects/Popliteal Stent/ExpandedStentSteel.png" 
     style="max-width: 100%;"/> 
  <h4>Nitinol Stent</h4>
  <img src="3d Modelling Projects/Popliteal Stent/ExpansionStentNitinol.png" 
     style="max-width: 100%;"/> 
  <img src="3d Modelling Projects/Popliteal Stent/ExpandedStentNitinol.png" 
     style="max-width: 100%;"/> 
  <h4>Stent Stress Comparison</h4>
  <img src="3d Modelling Projects/Popliteal Stent/MatStressCompGraph.png" 
     style="max-width: 100%;"/> 
</div>

<div id="2" class="tabcontent">
  <h2>Electrodeposition System</h2>
  <p>Design an electrodeposition system for use on silicon chips</p>
 <img src="3d Modelling Projects/Electrodeposition System/FullSystem.png" 
     style="max-width: 100%;"/>
 <p></p>
 
 <p>Click to expand for images</p>
<button class="accordion" >Renderings</button>
<div class="panel">
  <h2>Renderings</h2>
  <h3>Rotating Cathode Holder</h3>
  <img src="3d Modelling Projects/Electrodeposition System/Cathode render.png"  
     style="max-width: 100%;"/>
  <img src="3d Modelling Projects/Electrodeposition System/Cathode open.png" 
     style="max-width: 100%;"/> 

  <h3>Anode Basket</h3>
  <img src="3d Modelling Projects/Electrodeposition System/Anode Render.png" 
     style="max-width: 100%;"/>
</div>

<button class="accordion" >Drawings</button>
<div class="panel">
      <h2>Drawings</h2>
      <img src="3d Modelling Projects/Electrodeposition System/CathodeAssembly.png" 
     style="max-width: 100%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/TopDraw.png" 
     style="max-width: 100%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/ClaspDraw.png" 
     style="max-width: 100%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/PinDraw.png" 
     style="max-width: 100%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/RingDraw.png" 
     style="max-width: 100%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/FoamDraw.png" 
     style="max-width: 100%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/CaseDraw.png" 
     style="max-width: 100%;"/>
     <img src="3d Modelling Projects/Electrodeposition System/ShaftDraw.png" 
     style="max-width: 100%;"/>
 </div>
</div>
<div id="3" class="tabcontent">
  <h2>Guitar Strummer</h2>
  <p>Develop a four bar linkage system for a specific purpose. A guitar strummer was chosen.</p>
  <h3>Motion Study of Part</h3>
  <img src="3d Modelling Projects/Guitar Strummer/MS.gif" 
     style="max-width: 100%;"/>
  <h3>Orthographic Projection of Rocker Part</h3>
  <img src="3d Modelling Projects/Guitar Strummer/rocker.png" 
     style="max-width: 100%;"/>



</div>

<div id="4" class="tabcontent">
  <h2>Mars Rover Wheel</h2>
  <p>Who we are and what we do.</p>
</div> 

<div id="5" class="tabcontent">
  <h2>Miscellaneous Renders</h2>
  <p></p>
   <div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div class="mySlides">
    <div class="numbertext">1 / 5</div>
    <img src="3d Modelling Projects/Miscellaneous Renders/Bridge Scene.png" style="width:100%">
    <div class="text">Under Bridge Scene</div>
  </div>

  <div class="mySlides">
    <div class="numbertext">2 / 5</div>
        <img src="3d Modelling Projects/Miscellaneous Renders/Sand.png" style="width:100%">
    <div class="text">Desert Scene</div>
  </div>

  <div class="mySlides">
    <div class="numbertext">3 / 5</div>
        <img src="3d Modelling Projects/Miscellaneous Renders/Hammer driver.png" style="width:100%">
    <div class="text">Hammer and Screwdriver Render</div>
  </div>

<div class="mySlides">
    <div class="numbertext">4 / 5</div>
        <img src="3d Modelling Projects/Miscellaneous Renders/moon island.png" style="width:100%">
    <div class="text">Moonlit Island Scene</div>
  </div>
  <div class="mySlides">
    <div class="numbertext">5 / 5</div>
        <img src="3d Modelling Projects/Miscellaneous Renders/table top.png" style="width:100%">
    <div class="text">Tavern Table Top Render</div>
  </div>
  <!-- Next and previous buttons -->
  <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
  <a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>
<!-- The dots/circles -->
<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span>
  <span class="dot" onclick="currentSlide(2)"></span>
  <span class="dot" onclick="currentSlide(3)"></span>
  <span class="dot" onclick="currentSlide(4)"></span>
  <span class="dot" onclick="currentSlide(5)"></span>
</div>

</div> 

</html>

