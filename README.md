<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Hi, I'm Kim!</title>
<!-- Load an icon library to show a hamburger menu (bars) on small screens -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
/* Pink theme */
:root {
  --pink: #ff8bbd;
  --light-pink: #ffaac4;
  --dark-pink: #ff3d6b;
  --white: #ffffff;
  --black: #000000;
}

/* Add a pink background color to the top navigation */
.topnav {
  background-color: var(--pink);
  overflow: hidden;
}

/* Style the links inside the navigation bar */
.topnav a {
  float: left;
  display: block;
  color: var(--white);
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

/* Change the color of links on hover */
.topnav a:hover {
  background-color: var(--light-pink);
  color: var(--black);
}

/* Add an active class to highlight the current page */
.topnav a.active {
  background-color: var(--dark-pink);
  color: var(--white);
}

/* Hide the link that should open and close the topnav on small screens */
.topnav .icon {
  display: none;
}

/* When the screen is less than 600 pixels wide, hide all links, except for the first one ("Logo"). Show the link that contains should open and close the topnav (.icon) */
@media screen and (max-width: 600px) {
  .topnav a:not(:first-child) {display: none;}
  .topnav a.icon {
    float: right;
    display: block;
  }
}

/* The "responsive" class is added to the topnav with JavaScript when the user clicks on the icon. This class makes the topnav look good on small screens (display the links vertically instead of horizontally) */
@media screen and (max-width: 600px) {
  .topnav.responsive {position: relative;}
  .topnav.responsive a.icon {
    position: absolute;
    right: 0;
    top: 0;
  }
  .topnav.responsive a {
    float: none;
    display: block;
    text-align: left;
  }
}

/* Pink theme for the rest of the page */
body {
  background-color: var(--white);
  color: var(--black);
}

h1, h2, h3 {
  color: var(--dark-pink);
}

a {
  color: var(--dark-pink);
}

a:hover {
  color: var(--light-pink);
}

hr {
  border-color: var(--dark-pink);
}
</style>
</head>	
<body>

<!-- Top Navigation Menu -->
<div class="topnav" id="myTopnav">
  <a href="#home" class="active">Logo</a>
  <!-- Navigation links (hidden by default) -->
  <div id="myLinks">
    <a href="#news">News</a>
    <a href="#contact">Contact</a>
    <a href="#about">About</a>
  </div>
  <!-- "Hamburger menu" / "Bar icon" to toggle the navigation links -->
  <a href="javascript:void(0);" class="icon" onclick="myFunction()">
    <i class="fa fa-bars"></i>
  </a>
</div>

<!-- Heading 1, your most important heading, starts here -->
<h1>Hi, I'm Kim!</h1>
<!-- Heading 1 finishes here -->

<hr>
<img src="ankor2013.jpeg" alt="Girl in a jacket" width="800" height="600">
<h2>About me</h2>

<p>If you like tacos, puppies, Zamrock and green - let's be besties!</p>   

<p>Moved back to London in 2015 after semi hitchhiking through Asia for two years, so if you are planning on going, hit me up. I may know a few hidden gems (if I can still remember)</p>

<p>Free Palestine!</p>

<h2>How to spend time on the web, without using socials</h2>

<!--edit the links and the URLs below for your favourite sites -->
<ol>
    <li><a href="https://www.mapcrunch.com"> If you like exploring random places </a></li>
    <li><a href="https://berghaintrainer.com"> Can you make it into Berghain? </a></li>
    <li><a href="http://www.staggeringbeauty.com"> Fun! </a></li>
</ol>

<script>
/* Toggle between adding and removing the "responsive" class to topnav when the user clicks on the icon */
function myFunction() {
  var x = document.getElementById("myTopnav");
  if (x.className === "topnav") {
    x.className += " responsive";
  } else {
    x.className = "topnav
