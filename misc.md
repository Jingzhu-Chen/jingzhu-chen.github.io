---
layout: misc
---

# A little corner for what I find fascinating ✨

## Podcast 🎙️:

<div class="publications">
<ol class="bibliography">

{% for podcast in site.data.podcast.main %}

<li>
<div class="pub-row" style="align-items: flex-start; padding: 8px 0;">
  <img src="{{ podcast.image }}" class="podcast-cover" alt="{{ podcast.podcast_name }}" />
  <div class="podcast-info">
    <div class="podcast-name">
      <a href="{{ podcast.link }}" target="_blank" rel="noopener">{{ podcast.podcast_name }}</a>
    </div>
    {% if podcast.recommend_episodes %}
    <div class="episode-label">My Personal Recommendation</div>
    <ul class="episode-list">
      {% for ep in podcast.recommend_episodes %}
      <li><a href="{{ ep.link }}" target="_blank" rel="noopener">{{ ep.name }}</a></li>
      {% endfor %}
    </ul>
    {% endif %}
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>

## 🐈 🐈 🐈 ......

<div class="publications">
<ol class="bibliography">

</ol>
</div>
