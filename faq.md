---
layout: default
title: FAQ
permalink: /faq/
---
<div class="container">
<article class="page">
<h1>{{ page.title }}</h1>
<h4>General</h4>
<div name="posts">
	{% assign faqlist = (site.faqs | where: "category" , "General" | sort: "number") %}
	{% for faq in faqlist %}
      <h5><a href="#{{ faq.urlname }}">{{ forloop.index }} {{ faq.title }}</a></h5>
	{% endfor %}
</div>
<h4>Ecgine Basics</h4>
<div name="posts">
	{% assign faqlist = (site.faqs | where: "category" , "Ecgine Basics" | sort: "number") %}
	{% for faq in faqlist %}
 		<h5><a href="#{{ faq.urlname }}">{{ forloop.index }} {{ faq.title }}</a></h5>
	{% endfor %}
</div>
<h4>Security</h4>
<div name="posts">
	{% assign faqlist = (site.faqs | where: "category" , "Security" | sort: "number") %}
	{% for faq in faqlist %}
      <h5><a href="#{{ faq.urlname }}">{{ forloop.index }} {{ faq.title }}</a></h5>
	{% endfor %}
</div>
<h4>Others</h4>
<div name="posts">
	{% assign faqlist = (site.faqs | where: "category" , "Others" | sort: "number") %}
	{% for faq in faqlist %}
      <h5><a href="#{{ faq.urlname }}">{{ forloop.index }} {{ faq.title }}</a></h5>
	{% endfor %}
</div>


<h4>General</h4>
<div name="postsDetail">
	{% assign faqlist = (site.faqs | where: "category" , "General" | sort: "number") %}
	{% for faq in faqlist %}
       	<div id="{{ faq.urlname }}">
       		<h5>{{ forloop.index }} {{ faq.title }}</h5>
       		{{faq.content}}
   		</div>
	{% endfor %}
</div>

<h4>Ecgine Basics</h4>
<div name="postsDetail">
	{% assign faqlist = (site.faqs | where: "category" , "Ecgine Basics" | sort: "number") %}
	{% for faq in faqlist %}
       	<div id="{{ faq.urlname }}">
       		<h5>{{ forloop.index }} {{ faq.title }}</h5>
       		{{faq.content}}
   		</div>
	{% endfor %}
</div>

<h4>Security</h4>
<div name="postsDetail">
	{% assign faqlist = (site.faqs | where: "category" , "Security" | sort: "number") %}
	{% for faq in faqlist %}
       	<div id="{{ faq.urlname }}">
       		<h5>{{ forloop.index }} {{ faq.title }}</h5>
       		{{faq.content}}
   		</div>
	{% endfor %}
</div>

<h4>Others</h4>
<div name="postsDetail">
	{% assign faqlist = (site.faqs | where: "category" , "Others" | sort: "number") %}
	{% for faq in faqlist %}
       	<div id="{{ faq.urlname }}">
       		<h5>{{ forloop.index }} {{ faq.title }}</h5>
       		{{faq.content}}
   		</div>
	{% endfor %}
</div>
</article>
</div>