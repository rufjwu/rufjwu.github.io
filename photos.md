---
layout: page
title: Photos
---
## Photos

<!-- ![Test](/img/img-test.png "Test") -->
<html>
	{% for image in site.static_files %}
		{% if image.path contains 'photos' %}
		<img src="{{ site.base_url }}{{ image.path }}" alt="image" />
		{% endif %}
	{% endfor %}
</html>