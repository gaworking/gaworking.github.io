---
layout: page
title: Drums - Live Peformance Recording
songs:
  - "All Wrong": assets/mp3/02-All-Wrong.mp3
  - "Imaginary Song": assets/mp3/04-Imaginary-Song.mp3
  - "Honey White": assets/mp3/10-Honey-White.mp3
---

{% for song_hash in page.songs %}
{% for song in song_hash %}

**{{ song[0] }}**

<audio controls="controls">
<source src="{{ song[1] }}" />  
</audio> 
<br/>
{% endfor %}
{% endfor %}
