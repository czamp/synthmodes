---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

Collection of mobile-friendly synthesizer cheat sheets.<br /><br />

{% assign sorted_pages = site.pages | sort: 'title' %}

{%- for my_page in sorted_pages -%}
  {%- if my_page.title -%}
  <a class="page-link" href="{{ my_page.url | relative_url }}">{{ my_page.title | escape }}</a><br />
  {%- endif -%}
{%- endfor -%}
