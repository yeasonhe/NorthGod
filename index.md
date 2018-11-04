---
layout: default
---

{% for post in site.posts %}
*   {{ post.date|date_to_string }} [{{ post.title }}]({{site.baseurl}}{{post.url}})
{% endfor %}

[Link to another page](./another-page.html).

* * *

```
Thanks for your visiting
```
