---
title: Twain House Stories
layout: gayrodeo
permalink: /twain-house-stories.html
type: landing
---

Stories to come! 

{% for conversation in site.data.conversation-filters %}
<div id="convo-{{ forloop.index }}"></div>
<script id="{{ conversation.tag }}" type="html">
    <div class="row justify-content-center">
        <div class="card col-md-4 border-0 bg-dark mt-5 mb-3">
            <h1 class="text-black bg-white border-0 conversation py-3 px-3 text-center {{ conversation.tag }}">{{ conversation.question }}</h1>
        </div>
    </div>
    <div class="container-fluid timeline mb-5 mt-n3">

        {% for clip in site.data.master-conversations %}
        {% if clip.tag contains conversation.tag %}

            <div class="row {{ conversation.tag }} my-4">
                <div class="{{ clip.tag }} card col-md-4 my-3 my-md-0 border border-secondary text-black {% cycle 'offset-md-2 left-text-box ', 'offset-md-6 right-text-box ' %}" data-aos="{% cycle 'zoom-in-right', 'zoom-in-left'%}">
                    <div class="card-body">
                            <p class="card-text words">{{ clip.comments }}</p>
                            <p class="text-right name">-{{ clip.firstname }} {{ clip.lastname }}</p>
                    </div>
                </div>      
            </div>        

        {% endif %}
        {% endfor %}

    </div>  
</script>
{% endfor %}

<div class="row justify-content-center">
    <div class="col-md-3 text-center">
        <button class="btn btn-lg btn-warning my-4" id="more">New Conversation</button>
    </div>
</div>
    