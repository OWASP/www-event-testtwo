---

title: Keynotes
permalink: keynotes/
layout: event_noheader

---

<div class="keynote-full">
	
	<ul>
	{% for speaker in site.data.keynotespeakers %}
		{% if speaker.name %}
		<li>
			<a name="{{speaker.name}}">
			<img style="background-image: url(/www-event-testtwo/assets/images/keynotes/{{speaker.image | default: 'owasp_logo.png'}});{{speaker.style}};"></a>
			<h4><a name="{{speaker.name}}">{{speaker.name}}</a></h4>
			<p>
				{{speaker.bio}}
			</p>
		</li>
		{% endif %}
	{% endfor %}
	</ul>

</div>