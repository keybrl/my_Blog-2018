---
title: "项目"
landing-title: "优雅的代码"
layout: landing
description: 'Lorem ipsum dolor sit amet nullam consequa<br />sed veroeros. tempus adipiscing nulla.'
image: images/pic07.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h2>Sed amet aliquam</h2>
		</header>
		<p>Nullam et orci eu lorem consequat tincidunt vivamus et sagittis magna sed nunc rhoncus condimentum sem. In efficitur ligula tate urna. Maecenas massa vel lacinia pellentesque lorem ipsum dolor. Nullam et orci eu lorem consequat tincidunt. Vivamus et sagittis libero. Nullam et orci eu lorem consequat tincidunt vivamus et sagittis magna sed nunc rhoncus condimentum sem. In efficitur ligula tate urna.</p>
	</div>
</section>

<!-- Two -->
<section id="two" class="spotlights">
  {% for post in site.posts %}
  {% if post.layout == 'project' %}
    <section>
      <a href="{{ post.url  | relative_url }}" class="image">
        <img src="{{ site.assets_url }}/{{ post.image }}" alt="" data-position="center center" />
      </a>
      <div class="content">
        <div class="inner">
          <header class="major">
            <h3>{{ post.title }}</h3>
          </header>
          <p>{{ post.excerpt }}</p>
          <ul class="actions">
            <li><a href="{{ post.url  | relative_url }}" class="button">了解更多</a></li>
          </ul>
        </div>
      </div>
    </section>
  {% endif %}
  {% endfor %}
</section>

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
