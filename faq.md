---
layout: default
title: FAQ
permalink: /faq/
---
<div class="container">
<article class="page">
<h1>{{ page.title }}</h1>
<h3>General</h3>
<div name="posts">
	{% assign faqlist = (site.faqs | where: "category" , "General" | sort: "number") %}
	{% for faq in faqlist %}
      <h4><a href="#{{ faq.urlname }}">{{ forloop.index }} {{ faq.title }}</a></h4>
	{% endfor %}
</div>
<h3>Ecgine Basics</h3>
<div name="posts">
	{% assign faqlist = (site.faqs | where: "category" , "Ecgine Basics" | sort: "number") %}
	{% for faq in faqlist %}
 		<h4><a href="#{{ faq.urlname }}">{{ forloop.index }} {{ faq.title }}</a></h4>
	{% endfor %}
</div>
<h3>Security</h3>
<div name="posts">
	{% assign faqlist = (site.faqs | where: "category" , "Security" | sort: "number") %}
	{% for faq in faqlist %}
      <h4><a href="#{{ faq.urlname }}">{{ forloop.index }} {{ faq.title }}</a></h4>
	{% endfor %}
</div>
<h3>Others</h3>
<div name="posts">
	{% assign faqlist = (site.faqs | where: "category" , "Others" | sort: "number") %}
	{% for faq in faqlist %}
      <h4><a href="#{{ faq.urlname }}">{{ forloop.index }} {{ faq.title }}</a></h4>
	{% endfor %}
</div>


<h3>General</h3>
<div name="postsDetail">
	{% assign faqlist = (site.faqs | where: "category" , "General" | sort: "number") %}
	{% for faq in faqlist %}
       	<div id="{{ faq.urlname }}">
       		<h4>{{ forloop.index }} {{ faq.title }}</h4>
       		{{faq.content}}
   		</div>
	{% endfor %}
</div>

<h3>Ecgine Basics</h3>
<div name="postsDetail">
	{% assign faqlist = (site.faqs | where: "category" , "Ecgine Basics" | sort: "number") %}
	{% for faq in faqlist %}
       	<div id="{{ faq.urlname }}">
       		<h4>{{ forloop.index }} {{ faq.title }}</h4>
       		{{faq.content}}
   		</div>
	{% endfor %}
</div>

<h3>Security</h3>
<div name="postsDetail">
	{% assign faqlist = (site.faqs | where: "category" , "Security" | sort: "number") %}
	{% for faq in faqlist %}
       	<div id="{{ faq.urlname }}">
       		<h4>{{ forloop.index }} {{ faq.title }}</h4>
       		{{faq.content}}
   		</div>
	{% endfor %}
</div>

<h3>Others</h3>
<div name="postsDetail">
	{% assign faqlist = (site.faqs | where: "category" , "Others" | sort: "number") %}
	{% for faq in faqlist %}
       	<div id="{{ faq.urlname }}">
       		<h4>{{ forloop.index }} {{ faq.title }}</h4>
       		{{faq.content}}
   		</div>
	{% endfor %}
</div>
</article>
</div>