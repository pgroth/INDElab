---
layout: default
permalink: /people/
title: people
description: lab members
---

{% if site.data.people %}
<div class="post-content clearfix">
    {% for member in site.data.people %}
     <div class="profile col one left" >
        <img src="{{member.img | prepend: site.baseurl | prepend: site.url }}"/>
        <br>
        <a href="{{ member.url }} ">{{ member["name"] }}</a>

    </div>
    {% endfor %}

</div>
{% endif %}
