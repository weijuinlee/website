---
permalink: "/team"
layout: page
title: "The Team"
---

<p>We are the team that brings you the best experience in the field of Computer Science.</p>

<p>
	Interested in joining us? At our October STMU (an <abbr title="Extraordinary General Meeting">EGM</abbr>) we will be electing the:
	freshers' rep, third year rep, and the fourth year rep.
</p>

{% for cohort in site.data.committee %}
	<h2>{{ cohort.year }}</h2>

	<ul>
		{% for member in cohort.members %}
			<li>
				<strong>{{ member.name }}</strong> - <em>{{ member.role }}</em>
			</li>
		{% endfor %}
	</ul>
{% endfor %}