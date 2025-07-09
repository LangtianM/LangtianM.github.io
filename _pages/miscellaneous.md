---
layout: page
title: Miscellaneous
nav_order: 4
permalink: /miscellaneous/
nav: true
---

Thanks for visiting this page! Beside my academic life, I'm also interested in photography, literature and philosophy. I would like to share some of my photography works here.

## Life in Madison

<div style="display: flex; overflow-x: scroll; width: 100%; padding: 10px; gap: 10px;">
    {% assign image_files = site.static_files | where_exp: "file", "file.path contains '/photography/Madison/' and file.extname == '.jpg'" %}
    {% for image in image_files %}
    <img src="{{ image.path | relative_url }}" alt="Madison {{ forloop.index }}" style="height: 200px;"/>
    {% endfor %}
</div>

## The Winter of Madison

<div style="display: flex; overflow-x: scroll; width: 100%; padding: 10px; gap: 10px;">
    {% assign image_files = site.static_files | where_exp: "file", "file.path contains '/photography/Madison_Winter/' and file.extname == '.jpg'" | reverse %}
    {% for image in image_files %}
    <img src="{{ image.path | relative_url }}" alt="Winter {{ forloop.index }}" style="height: 200px;"/>
    {% endfor %}
</div>

## Travels

<div style="display: flex; overflow-x: scroll; width: 100%; padding: 10px; gap: 10px;">
    {% assign image_files = site.static_files | where_exp: "file", "file.path contains '/photography/Travels/'" %}
    {% assign image_files = image_files | where_exp: "file", "file.extname == '.jpg' or file.extname == '.jpeg' or file.extname == '.JPG'" %}
    {% for image in image_files %}
    <img src="{{ image.path | relative_url }}" alt="Travels {{ forloop.index }}" style="height: 200px;"/>
    {% endfor %}
</div>

## Chicago

<div style="display: flex; overflow-x: scroll; width: 100%; padding: 10px; gap: 10px;">
    {% assign image_files = site.static_files | where_exp: "file", "file.path contains '/photography/Chicago/' and file.extname == '.jpg'" %}
    {% for image in image_files %}
    <img src="{{ image.path | relative_url }}" alt="Chicago {{ forloop.index }}" style="height: 200px;"/>
    {% endfor %}
</div>


## Xi'an

<div style="display: flex; overflow-x: scroll; width: 100%; padding: 10px; gap: 10px;">
    {% assign xian_path = "/photography/Xi'an/" %}
    {% assign image_files = site.static_files | where_exp: "file", "file.path contains xian_path" %}
    {% assign image_files = image_files | where_exp: "file", "file.extname == '.jpg'" | reverse %}
    {% for image in image_files %}
    <img src="{{ image.path | relative_url }}" alt="Xi'an {{ forloop.index }}" style="height: 200px;"/>
    {% endfor %}
</div>

## Clouds and Sunsets

<div style="display: flex; overflow-x: scroll; width: 100%; padding: 10px; gap: 10px;">
    {% assign image_files = site.static_files | where_exp: "file", "file.path contains '/photography/Clouds_and_Sunsets/'" %}
    {% assign image_files = image_files | where_exp: "file", "file.extname == '.jpg' or file.extname == '.jpeg' or file.extname == '.JPG'" | reverse %}
    {% for image in image_files %}
    <img src="{{ image.path | relative_url }}" alt="Clouds and Sunsets {{ forloop.index }}" style="height: 200px;"/>
    {% endfor %}
</div>

## Others

<div style="display: flex; overflow-x: scroll; width: 100%; padding: 10px; gap: 10px;">
    {% assign image_files = site.static_files | where_exp: "file", "file.path contains '/photography/Others/'" %}
    {% assign image_files = image_files | where_exp: "file", "file.extname == '.jpg' or file.extname == '.jpeg' or file.extname == '.JPG'" %}
    {% for image in image_files %}
    <img src="{{ image.path | relative_url }}" alt="Others {{ forloop.index }}" style="height: 200px;"/>
    {% endfor %}
</div>
