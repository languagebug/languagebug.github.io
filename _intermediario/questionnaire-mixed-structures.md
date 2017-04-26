---
title: "Questionnaire: Mixed Structure"
layout: revealjs-default
category: structure
---

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