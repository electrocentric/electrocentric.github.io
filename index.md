---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Projects
---
<div class="project-list">
{% for post in site.posts %}
    <article class="project-thumbnail">
	  
	  <div class="project-image" style="background-image:url('{{ post.projectimage }}')">
		<a href="{{ post.url }}">
			<div class="project-title">
				<h2>{{ post.title }}</h2>
			</div>
			<img src="/assets/companies/{{post.company}}-350.png" class="project-company">
		</a>
	  </div>
    </article>
{% endfor %}
</div>