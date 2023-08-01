---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: EV CHARGE Model Documentation
---

Identifying the appropriate charging infrastructure to deploy at the right pace and location is key to achieving the zero-mission vehicle adoption needed to reach our climate goals. Since this is a complex task, the ICCT developed EV CHARGE: a Python-based model to assess charging infrastructure needs for light-duty vehicles (2 and 3 wheelers, passenger cars, and light commercial vehicles) at any given scale: from local (e.g. city district level) to supra-national (e.g. European Union level), for any market and at any time horizon, based on a list of required inputs. This model is intended for in-house utilization only and streamlines and standardizes charging needs assessment analyses. After describing the motivation for deploying such a model, the authors outline the methodology, present the data inputs and outputs, and finish with the provision of use cases.

## Versions

EV CHARGE is under continuing development. Documentation of all versions after v.1.0 can be found here.

{% assign pages = site.pages | sort: "title" | reverse %}
{% for page in pages %}
{% if page.dir contains '/versions/' and page.title contains 'EV CHARGE v'%}
<li><a class="page-link" href="{{ page.url | relative_url }}">{{ page.title | escape }}</a></li>
{% endif %}
{% endfor %}
