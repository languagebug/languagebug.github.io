---
title: "Lots of questions"
layout: revealjs-default
category: structure
---

<section>
<h1>Lots of questions</h1>
</section>

<section>
<ol>
{% for item in site.beginner %}
    {% if item.category == "questions" %}
      <li>{{ item.structure }} ____ ?</li>
    {% endif %}
{% endfor %}
</ol>
</section>

{% for i in (1..10) %}
<section>
<ol>
{% for item in site.beginner %}
		{% if item.category == "questions" %}
			<li>{{ item.structure }} <u>{{ item.examples[i] }}</u>?</li>
		{% endif %}
{% endfor %}
</ol>
</section>
{% endfor %}