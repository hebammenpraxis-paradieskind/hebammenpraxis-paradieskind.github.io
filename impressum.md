---
layout: page
title: Impressum
background: white
sitemap: false
---

# Impressum

--- 

<div class="row">
    <div class="col-12 mx-auto text-left">

    <div style="margin-bottom: 1em;">
        {% for paragraph in site.data.sitetext[site.locale].contact_simple.address %}
        <div class="large text-muted address">{{ paragraph | markdownify }}</div>
        {% endfor %}
    </div>

    {% for person in site.data.sitetext[site.locale].team.people %}
    <div class="large text-muted address">
        <p>
        <i class="fas fa-mobile-alt" aria-hidden="true"></i>
        {{ person.name }}:
        <a href="tel:{{ person.telephone }}">{{
            person.telephone }}</a>
        </p>
    </div>
    {% endfor %}

    <div class="large text-muted address">
        <p>
        <i class="fas fa-envelope" aria-hidden="true"></i>
        <a href="mailto:{{ site.data.sitetext[site.locale].contact_simple.email }}">{{
            site.data.sitetext[site.locale].contact_simple.email }}</a>
        </p>
    </div>

    <div class="large text-muted address">
    <p><b>IK:</b> 451607857</p>
    </div>    
</div>

