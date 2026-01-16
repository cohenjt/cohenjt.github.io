---
permalink: /youth-education/
title: "Youth Education"
header:
    overlay_image: "/assets/images/seaheader.jpeg"
---

<style>
.accordion-header {
  background-color: #f1f1f1;
  color: #333;
  cursor: pointer;
  padding: 12px;
  border: 2px solid #ddd;
  border-radius: 4px;
  margin-top: 1em;
  font-size: 1.2em;
  font-weight: bold;
  transition: background-color 0.3s ease;
}

.accordion-header:hover {
  background-color: #e0e0e0;
}

.accordion-header.active {
  background-color: #ccc;
}

.accordion-content {
  display: none;
  background-color: #f9f9f9;
  border: 2px solid #ddd;
  border-top: none;
  border-radius: 0 0 4px 4px;
  padding: 12px;
  margin-bottom: 1em;
}

.accordion-content.active {
  display: block;
}

.content-row {
  display: flex;
  align-items: center;
  gap: 15px;
}

.content-image {
  flex: 0 0 25%;
  max-width: 25%;
}

.content-image img {
  width: 100%;
  height: auto;
  border-radius: 4px;
  border: 2px solid #ddd;
}

.content-text {
  flex: 0 0 75%;
  max-width: 75%;
}
</style>

<script>
function setupAccordion() {
  const headers = document.querySelectorAll('.accordion-header');
  
  headers.forEach(header => {
    header.addEventListener('click', function() {
      const content = this.nextElementSibling;
      
      // Close all other accordion items
      headers.forEach(h => {
        if (h !== this) {
          h.classList.remove('active');
          h.nextElementSibling.classList.remove('active');
        }
      });
      
      // Toggle current accordion item
      this.classList.toggle('active');
      content.classList.toggle('active');
    });
  });
}

document.addEventListener('DOMContentLoaded', setupAccordion);
</script>

# Youth Education

<div class="accordion-header">Middle School Ultimate Frisbee Coach</div>
<div class="accordion-content">
  <div class="content-row">
    <div class="content-image">
      <img src="/assets/images/acorn.jpg" alt="Ultimate Frisbee">
    </div>
    <div class="content-text">
      I coach the middle school ultimate frisbee team at the Seattle Waldorf school. I work with students to develop their athletic skills and teamwork, emphasizing sportsmanship and 
    </div>
  </div>
</div>

<div class="accordion-header">Substitute Teacher</div>
<div class="accordion-content">
  <div class="content-row">
    <div class="content-text">
      During a break between my Ph.D. and my postdoc, I occasionally worked as a substitute teacher at the Bush School in Seattle, WA. I primarily tought middle school and high school math, and filled in for a few other classes as needed.
    </div>
    <div class="content-image">
      <img src="/assets/images/acorn.jpg" alt="Teaching">
    </div>
  </div>
</div>
