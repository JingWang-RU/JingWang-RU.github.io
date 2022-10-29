---
layout: page
permalink: /teaching/
title: photography
description: Use photos to record memories.
nav: true
nav_order: 5
---
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="/assets/img/spain_1.jpg" title="example image" class="rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="/assets/img/uk_3.jpg" title="example image" class="img-fluid rounded z-depth-1" style="object-fit:none;width:800px; height:53px;border: solid 1px #CCC" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="/assets/img/uk_9.jpg" title="example image" class="img-fluid rounded z-depth-1" style="object-fit:none;width:800px; height:53px;border: solid 1px #CCC" %}
    </div>
</div>
<div class="caption">
    The left photo is taken in a museum of seville, Spain. Middle is a Buddha statue from British museum. The right is taken on london bridge.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/california.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This photo is in California.
</div>



<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/nj_3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/nj_2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left, the parking lot of Rutgers University, Pistataway; Right, United Nations Headquarters in NYC.
</div>


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/spain_2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/ny_2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left is Cadiz, Spain; On the right is Empire State building.
</div>


<div class="container">
  <div style="text-align:center">
    <h2>Contact Me</h2>
    <p>Leave me a message:</p>
  </div>
  <div class="row">
   <!--  <div class="column">
      <img src="/assets/img/4.jpg" style="width:100%">
    </di -->v>
    <div class="column">
      <form action="mailto:janelmm@163.com">
        <label for="fname">First Name</label>
        <input type="text" id="fname" name="firstname" placeholder="Your name..">
        <label for="lname">Last Name</label>
        <input type="text" id="lname" name="lastname" placeholder="Your last name..">
        <label for="country">Continent</label>
        <select id="country" name="country">
        	<option value="asia">Asia</option>
          	<option value="africa">Africa</option>
          	<option value="autralia">Australia</option>
           	<option value="europe">Europe</option>
            <option value="middleeast">Middle East</option>
            <option value="northamerica">NorthAmerica</option>
            <option value="southamerica">South America</option>
		</select>
        <label for="subject">Subject</label>
        <textarea id="subject" name="subject" placeholder="Write something.." style="height:170px"></textarea>
        <input type="submit" value="Submit">
      </form>
    </div>
  </div>
</div>
