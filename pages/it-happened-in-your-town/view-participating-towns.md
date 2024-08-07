---
title: It Happened In Your Town
layout: about
permalink: /education.html
---
# It Happened In Your Town

In 2024, we’re celebrating the 150th birthday of The Mark Twain House with our city-wide digital exhibit “It Happened In Hartford.” But what was happening in the rest of the state in 1874? Connecticut teachers and students (grades 6-12 & undergrads) and local historical societies have selected objects and items to share what was happening in their town. It Happened In Your Town will allow students to engage with their community’s past and present, demonstrating the power of local history to tell national and global stories. 

{% for town in site.towns %}
- 	[{{ town.title }}]({{ town.permalink }}) by {{ town.author }}
{% endfor %}

<a href="{{ '/browse.html' | relative_url }}" class="btn btn-outline-primary">Browse Submittted Items</a>
<a href="{{ '/map.html' | relative_url }}" class="btn btn-outline-primary">View Map</a>
<a href="{{ '/timeline.html' | relative_url }}" class="btn btn-outline-primary">View Timeline</a>

**Interested in getting involved? Visit our [Get Involved]({{ "/getinvolved.html" | relative_url }}) page to learn more.**
