---
title: Publications
layout: landing
description: 'We research focused on the the algorithm and technology about CV & AI<br />Here are some featured publications.'
image: assets/images/pic07.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">


{% assign publications = site.publications | sort: "year" | reverse %}

{% for pub in publications %}
{% if pub.work-type == 'Paper' %}

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h2>journal</h2>
		</header>
		<p>"The systematic investigation into and study of materials and sources in order to establish facts and reach new conclusions"</p>
	</div>
</section>

<section id="two" class="spotlights">
	<section>
		<a href="generic.html" class="image">
			<img src="/assets/images/publications/{{ pub.ref-cover }}"  alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3> <a href="{% if pub.ref-doi %}http://dx.doi.org/{{ pub.ref-doi }}
            			{% else %}{{ pub.url | prepend: site.baseurl }}{% endif %}">
           				 {{ pub.ref-authors }} ({{ pub.ref-year }}).</a>
					</h3>
				</header>
				<p>
					{{ pub.ref-title }}. 
					<em>{{ pub.ref-journal}}</em>{% if pub.ref-vol %}, {{ pub.ref-vol }}{% endif %}. 
					{% if pub.ref-doi %}
					<a href="http://dx.doi.org/{{ pub.ref-doi }}">doi: {{ pub.ref-doi }}</a>
					{% endif %}
				</p>
				<!--ul class="actions">
					<li><a href="generic.html" class="button">Learn more</a></li>
				</ul-->
			</div>
		</div>
	</section>
</section>
{% endif %}
{% endfor %}

<!-- Two >
<section id="two" class="spotlights">
	<section>
		<a href="generic.html" class="image">
			<img src="{% link assets/images/pic08.jpg %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Orci maecenas</h3>
				</header>
				<p>Nullam et orci eu lorem consequat tincidunt vivamus et sagittis magna sed nunc rhoncus condimentum sem. In efficitur ligula tate urna. Maecenas massa sed magna lacinia magna pellentesque lorem ipsum dolor. Nullam et orci eu lorem consequat tincidunt. Vivamus et sagittis tempus.</p>
				<ul class="actions">
					<li><a href="generic.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section>
		<a href="generic.html" class="image">
			<img src="{% link assets/images/pic09.jpg %}" alt="" data-position="top center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Rhoncus magna</h3>
				</header>
				<p>Nullam et orci eu lorem consequat tincidunt vivamus et sagittis magna sed nunc rhoncus condimentum sem. In efficitur ligula tate urna. Maecenas massa sed magna lacinia magna pellentesque lorem ipsum dolor. Nullam et orci eu lorem consequat tincidunt. Vivamus et sagittis tempus.</p>
				<ul class="actions">
					<li><a href="generic.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section>
		<a href="generic.html" class="image">
			<img src="{% link assets/images/pic10.jpg %}" alt="" data-position="25% 25%" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Sed nunc ligula</h3>
				</header>
				<p>Nullam et orci eu lorem consequat tincidunt vivamus et sagittis magna sed nunc rhoncus condimentum sem. In efficitur ligula tate urna. Maecenas massa sed magna lacinia magna pellentesque lorem ipsum dolor. Nullam et orci eu lorem consequat tincidunt. Vivamus et sagittis tempus.</p>
				<ul class="actions">
					<li><a href="generic.html" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
</section-->

<!-- Three -->
<section id="three">
	<div class="inner">
		<header class="major">
			<h2>Massa libero</h2>
		</header>
		<p>Nullam et orci eu lorem consequat tincidunt vivamus et sagittis libero. Mauris aliquet magna magna sed nunc rhoncus pharetra. Pellentesque condimentum sem. In efficitur ligula tate urna. Maecenas laoreet massa vel lacinia pellentesque lorem ipsum dolor. Nullam et orci eu lorem consequat tincidunt. Vivamus et sagittis libero. Mauris aliquet magna magna sed nunc rhoncus amet pharetra et feugiat tempus.</p>
		<ul class="actions">
			<li><a href="generic.html" class="button next">Get Started</a></li>
		</ul>
	</div>
</section>

</div>
