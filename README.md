<html>
<head>
<style>
body {font-family: Arial;}

/* Style the tab */
.tab {
  overflow: hidden;
  border: 1px solid #ccc;
  background-color: #92EDE5;
}

/* Style the buttons inside the tab */
.tab button {
  background-color: inherit;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  transition: 0.3s;
  font-size: 17px;
}

/* Change background color of buttons on hover */
.tab button:hover {
  background-color: #ddd;
}

/* Create an active/current tablink class */
.tab button.active {
  background-color: #ccc;
}

/* Style the tab content */
.tabcontent {
  display: none;
  padding: 6px 12px;
  border: 1px solid #ccc;
  border-top: none;
}
</style>
</head>
<body>

<h2>Jamila's Henna Store</h2>
<p>Here to meet all your Henna needs for any occasion.</p>

<div class="tab">
  <button class="tablinks" onclick="opentab(event, 'About Us')">About Us</button>
  <button class="tablinks" onclick="opentab(event, 'Henna Styles')">Henna Styles</button>
  <button class="tablinks" onclick="opentab(event, 'Pricing')">Pricing</button>
</div>

<div id="About Us" class="tabcontent">
  <h3>About Us</h3>
  <p>We are a Henna Store based in Minneapolis within the Karmel Store. We add to the vibrant Somali Community and are excited to... </p>
</div>

<div id="Henna Styles" class="tabcontent">
  <h3>Henna Styles</h3>
  <p>Paris is the capital of France.</p>
</div>

<div id="Pricing" class="tabcontent">
  <h3>Pricing</h3>
  <p>Tokyo is the capital of Japan.</p>
</div>

<script>
function opentab(evt, tabname) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(tabname).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>

</body>
</html>
