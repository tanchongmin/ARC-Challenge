---
layout: directory
title: Directory Listing
---
{% assign sorted_pages = site.pages | sort: 'url' %}
{% assign filtered_pages = sorted_pages | where_exp: "page", "page.url != '/directory.html'" %}

{% assign sorted_posts = site.posts | sort: 'url' %}

{% assign all_items = sorted_pages | concat: sorted_posts %}
{% for item in all_items %}
  {% unless item.url contains 'directory.html' %}
    {% assign item_title = item.title | default: item.url %}
    {% assign page_entry = '{ "title": "' | append: item_title | append: '", "url": "' | append: item.url | append: '" }' %}
    {% capture page_entries %}{{ page_entries | default: '[]' | append: ',' | append: page_entry }}{% endcapture %}
  {% endunless %}
{% endfor %}
{% assign directory_json = '[' | append: page_entries | append: ']' %}
{% assign directory_data = directory_json | jsonify %}
{% assign page.items = directory_data %}
