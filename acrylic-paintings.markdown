---
title: "Acrylic Paintings"
layout: "normal"
keywords: "Linda Mezzetti, Melbourne, Australia, paintings"
description: "Acrylic Paintings"
---
<h2 class="text-center my-3 pt-4">Acrylic Paintings</h2>
<div class="mx-auto" style="width:100%;height:440px">
<div id="carouselCaptions" class="carousel slide carousel-fade pb-4" data-ride="carousel">
  <ol class="carousel-indicators">

<li class="active" data-target="#carouselCaptions" data-slide-to="0"></li>
{% for i in (0..2) %}
<li {% if i == '0' %}class="active" {% endif %} data-target="#carouselCaptions" data-slide-to="{{i}}"></li>
{% endfor %}
</ol>
<div class="carousel-inner">

{% for acrylic in site.data.acrylics %}
{% capture number %}{{ forloop.length }}{% endcapture %}
{% if acrylic.file == 0 %} 
<div class="carousel-item active">
<img style="height:400px;width:auto" src="{{"assets/img/acrylics/0.jpg" | relative_url }}" class="d-block w-100" />
<div style="bottom:-18px;" class="carousel-caption d-none d-md-block">
   <span style="padding:5px;color:black;background-color:white">Image {{forloop.index}} of {{number}}. Feel the Music - Acrylic and mixed media, 51 x 61cm</span>
   </div>
   </div>
{% else %}
<div class="carousel-item">
<img style="height:400px;width:auto" src="../assets/img/acrylics/{{acrylic.file}}.jpg" class="d-block w-100" />
   <div style="bottom:-18px;" class="carousel-caption d-none d-md-block">
   <span style="padding:5px;color:black;background-color:white">Image {{forloop.index}} of {{number}}. {{acrylic.title}} ({{acrylic.size}})</span>
   </div>
   </div>
{% endif %}

{% endfor %}
  </div>
  <a class="carousel-control-prev" href="#carouselCaptions" role="button" data-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="carousel-control-next" href="#carouselCaptions" role="button" data-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div><!-- end carousel -->
</div>
<!-- end width -->

