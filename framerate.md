---
layout: default
title: Framerate
---
<style>
@media only screen and (min-width: 800px) {
   .teaser {
	float: left;
	width: 33%;
	box-sizing: border-box;
	padding: 0 5px;}

li.teaser:before{background:none;}
li.teaser img {width: 254px;height: 254px;object-fit: cover;
 }
}

  </style>
<div id="articles">

 <h1 class="pageTitle">Framerate</h1>
 <div class="post">
 <blockquote>Framerate captures the moments that wouldn't be enough for a story but without them we wouldn't see the big picture</blockquote>
 </div>
 <ul class="posts noList">
 
    {% for post in site.framerates reversed | sort: 'date' %}
      <li class="teaser">
    {% if post.image %}<a class="post-link" href="{{ post.url | prepend: site.baseurl }}"><img src=" {{ '/uploads/' | prepend: site.baseurl | append: post.image }}"> </a> {% endif %}
    	<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
	   </li>
     {% endfor %}
    </ul>


</div>


  
 
