---
layout: archive
title: ""
permalink: /teaching/
author_profile: true
---

I teach undergraduate economics courses, including Principles of Economics, Principles of Microeconomics, and Intermediate Macroeconomics. Class sizes range from 15 to 120 students, with an average teaching evaluation of 4.5 out of 5.


## Courses Offered
<hr> <!-- This adds a horizontal line below the heading -->
Intermediate Macroeconomics  - ECO 3311 \\
Principles of Microeconomics - ECO 2301 \\
Principles of Microeconomics - ECO 2301 - Online \\
Principles of Economics - ECO 2305 \\
Principles of Economics - ECO 2305 - Online \\
MathCamp for first-year Ph.D. Students 


## Teaching Assistant
<hr> <!-- This adds a horizontal line below the heading -->
Economic Data Analysis I - ECO 3363 \\
Economic Data Analysis II - ECO 3364 \\
Principles of Economics - ECO 2305 \\
Environmental Economics - ECO 3336  \\
Game Theory - ECO 3305 \\
Intermediate Economic Theory - ECO 3312 \\
International Economics - ECO 3333  \\
Economic Tutoring Center 


Hear From My Students!
<hr> <!-- This adds a horizontal line below the heading -->
<style>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing: border-box}
body {font-family: Verdana, sans-serif; margin:0}

/* Slideshow container */
.slideshow-container {
  position: relative;
  background: #f1f1f1f1;
}

/* Slides */
.mySlides {
  display: none;
  padding: 60px;
  text-align: center;
}

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  margin-top: -30px;
  padding: 16px;
  color: #888;
  font-weight: bold;
  font-size: 18px;
  border-radius: 0 3px 3px 0;
  user-select: none;
}

/* Position the "next button" to the right */
.next {
  position: absolute;
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.8);
  color: white;
}

/* The dot/bullet/indicator container */
.dot-container {
    text-align: center;
    padding: 20px;
    background: #ddd;
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 10px;
  width: 10px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

/* Add a background color to the active dot/circle */
.active, .dot:hover {
  background-color: #717171;
}

/* Add an italic font style to all quotes */
q {font-style: italic;}

/* Add a blue color to the author */
.author {color: cornflowerblue;}

</style>

<div class="slideshow-container">
	
<div class="mySlides">
  <q>The professor, Mr. Jalal was the incredible with helping students in their own needed way. Between staying after class and office hours I think he has
helped out almost the entire class. Very organized and teaches at a great speed.</q>
</div>

<div class="mySlides">
  <q>Really wants you to learn and not just hand you work for a grade.</q>
</div>

<div class="mySlides">
  <q>Super kind and helpful guy. Very smart and always answers questions kindly. Very flexible.</q>
</div>

<div class="mySlides">
  <q>The most effective aspects were homework and the lectures. I got plenty of good practice from the homework and the lectures were interactive as he did practice problems
with us on the chalkboard.</q>
</div>
	
<div class="mySlides">
  <q>I think he cares deeply about his students and actually wants them to learn, contrary to other professors at the school. I appreciated his class although I seemed to struggle.</q>
</div>

<div class="mySlides">
  <q>He was a great professor and it felt like he knew what he was talking about and the way to teach it to the students.</q>
</div>

<div class="mySlides">
  <q>Your teaching was really helpful and help me understand concepts. Overall keep up the great work!!</q>
</div>

<div class="mySlides">
  <q>Nice and most understanding professor Ive ever had! Responds quickly to emails and easy to understand. Good lectures and good coverage on all course topics.</q>
</div>

<div class="mySlides">
  <q>Good and fair instructor who I respected and was fully engaged with the class</q>
</div>

<div class="mySlides">
  <q>Very nice instructor. Gave lots of opportunities for us to succeed and organized the class very well.</q>
</div>
	

<!-- Next and previous buttons -->
<a class="prev" onclick="plusSlides(-1)">&#10094;</a>
<a class="next" onclick="plusSlides(1)">&#10095;</a>

</div>

<div class="dot-container" id="dotContainer"></div>

<script>
let slideIndex = 1;
let totalSlides = 10;
let visibleDots = 5;
let autoPlayInterval = null; // store autoplay interval

showSlides(slideIndex);

// Next/Prev controls
function plusSlides(n) {
  showSlides(slideIndex += n);
}

// Dot controls
function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}

  // Hide all slides
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  // Show current slide
  slides[slideIndex-1].style.display = "block";  

  // Update dots
  updateDots();
}

function updateDots() {
  let dotContainer = document.getElementById("dotContainer");
  dotContainer.innerHTML = ""; // Clear existing dots

  // Calculate group
  let groupStart = Math.floor((slideIndex-1) / visibleDots) * visibleDots + 1;
  let groupEnd = Math.min(groupStart + visibleDots - 1, totalSlides);

  for (let i = groupStart; i <= groupEnd; i++) {
    let dot = document.createElement("span");
    dot.className = "dot";
    if (i === slideIndex) {
      dot.classList.add("active");
    }
    dot.setAttribute("onclick", "currentSlide(" + i + ")");
    dotContainer.appendChild(dot);
  }
}

/* Optional autoplay */
function startAutoPlay(interval=4000) {
  stopAutoPlay(); // clear existing interval
  autoPlayInterval = setInterval(() => {
    plusSlides(1);
  }, interval);
}
function stopAutoPlay() {
  if (autoPlayInterval) {
    clearInterval(autoPlayInterval);
    autoPlayInterval = null;
  }
}

// Start autoplay (every 4 seconds)
startAutoPlay(4000);

</script>
