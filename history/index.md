---
layout: default
title: Our History
description: Project history and biographies of team members
keywords: team
imagedir: /images/team/
---
#Our History

<!-- ###The Story So Far -->

##Meet the Team

<div>
{% for ci in site.team %}
<div class="panel">
    <div class="row">
    	<div class="medium-3 columns text-center">

        <h3>{{ ci.name }}</h3>
        <img src="{{page.imagedir}}{{ci.image}}"/>
        </div>
        <div class="medium-9 columns>">
        <h4><em>{{ci.job}}</em></h4>
        {{ ci.content | markdownify}}
        </div>
    </div>
</div>
{% endfor %}
</div>