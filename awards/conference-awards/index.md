---
layout: ieeevr-default
title: "Conference Award Winners"
---

<style>
    <style>* {
        box-sizing: border-box;
    }

    .exhibitors-center {
        margin: auto;
        width: 90%;
    }

    .exhibitors-row {
        display: flex;
        background-color: #00aeef;
        border-radius: 10px;
        padding: 10px;
    }

    .exhibitors-column {
        flex: 50%;
        padding: 20px;
        position: relative;
    }

    .styled-table {
        border-collapse: collapse;
        margin: 25px 0;
        font-size: 0.8em;
        font-family: sans-serif;
        /*min-width: 400px;*/
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
        display: table;
    }

    .styled-table thead tr {
        background-color: #00aeef;
        color: #ffffff;
        text-align: left;
    }

    .styled-table th,
    .styled-table td {
        padding: 12px 15px;
        width: 50%;
    }

    .styled-table tbody tr {
        border-bottom: 1px solid #dddddd;
    }

    .styled-table tbody tr:nth-of-type(even) {
        background-color: #f3f3f3;
    }

    .styled-table tbody tr:last-of-type {
        border-bottom: 2px solid #00aeef;
    }

    .styled-table tbody tr.active-row {
        font-weight: bold;
        color: #00aeef;
    }

    /* Collapsible */
    input[type='checkbox'] {
        display: none;
    }

    .wrap-collabsible {
        margin: 1.2rem 0;
    }

    .lbl-toggle {
        display: block;
        font-weight: bold;
        /* font-family: monospace; */
        font-size: 1rem;
        text-align: left;
        padding: 0.1rem;
        color: #00aeef;
        background: #ffffff;
        cursor: pointer;
        border-radius: 7px;
        transition: all 0.25s ease-out;
    }

    .lbl-toggle:hover {
        /*color: #FFF;*/
    }

    .lbl-toggle::before {
        content: ' ';
        display: inline-block;
        border-top: 5px solid transparent;
        border-bottom: 5px solid transparent;
        border-left: 5px solid currentColor;
        vertical-align: middle;
        margin-right: .7rem;
        transform: translateY(-2px);
        transition: transform .2s ease-out;
    }

    .toggle:checked+.lbl-toggle::before {
        transform: rotate(90deg) translateX(-3px);
    }

    .collapsible-content {
        max-height: 0px;
        overflow: hidden;
        transition: max-height .25s ease-in-out;
    }

    .toggle:checked+.lbl-toggle+.collapsible-content {
        max-height: 1500px;
    }

    .toggle:checked+.lbl-toggle {
        border-bottom-right-radius: 0;
        border-bottom-left-radius: 0;
    }

    .collapsible-content .content-inner {
        background: white;
        /* rgba(0, 105, 255, .2);*/
        border-bottom: 1px solid rgba(0, 105, 255, .45);
        border-bottom-left-radius: 7px;
        border-bottom-right-radius: 7px;
        padding: .5rem 1rem;
    }

    .collapsible-content p {
        margin-bottom: 0;
    }



    /* video container */
    .video-container {
        overflow: hidden;
        position: relative;
        width: 100%;
    }

    .video-container::after {
        padding-top: 56.25%;
        /* 75% if 4:3*/
        display: block;
        content: '';
    }

    .video-container iframe {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
    }

    /* Thumbnails box */
    .box {
        border-radius: 5px;
        padding: 20px;
    }

    .box:nth-child(even) {
        color: red;
    }

    .wrapper {
        display: grid;
        /* border: 1px solid #000; */
        grid-gap: 10px;
        grid-template-columns: repeat(auto-fill, 150px 30%);
    }

    .styled-table2 {
        border-collapse: collapse;
        margin: 25px 0;
        font-size: 0.8em;
        font-family: sans-serif;
        /*min-width: 400px;*/
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
        display: table;
        width: 50%;
        margin-left: auto;
        margin-right: auto;


    }

    .styled-table2 thead tr {
        background-color: #00aeef;
        color: #ffffff;
        text-align: left;
    }

    .styled-table2 th,
    .styled-table2 td {
        padding: 12px 15px;
        width: 50%;
    }

    .styled-table2 tbody tr {
        border-bottom: 1px solid #dddddd;
    }

    .styled-table2 tbody tr:nth-of-type(even) {
        background-color: #f3f3f3;
    }

    .styled-table2 tbody tr:last-of-type {
        border-bottom: 2px solid #00aeef;
    }

    .styled-table2 tbody tr.active-row {
        font-weight: bold;
        color: #00aeef;
    }

    img {
        display: block;
        margin-left: auto;
        margin-right: auto;
    }

    /*
    div {
        text-align: justify;
        text-justify: inter-word;
    }
    */

</style>


<h1>IEEE VR 2021 Conference Awards</h1>

<p>
    Blurb
</p>


<table class="styled-table" style="font-size: 0.9em; ">
    <tr>
        <th>Conference Awards</th>
    </tr>
    <tr>
        <td><strong><a href="#journal-best">TVCG - Best Journal Papers</a></strong></td>
    </tr>
</table>



<h2 id='journal-best' style="text-align: center; color: #00aeef;">TVCG - Best Journal Papers</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Journal' %}
        {% if item.award == 'Best Paper' %}
        
            {% for j in site.data.journalpapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='journal-honorable' style="text-align: center; color: #00aeef;">TVCG - Honorable Mentions</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Journal' %}
        {% if item.award == 'Honorable Mention' %}
        
            {% for j in site.data.journalpapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='journal-nominees' style="text-align: center; color: #00aeef;">TVCG - Best Journal - Nominees</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Journal' %}
        {% if item.award == 'Nominee' %}
        
            {% for j in site.data.journalpapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='conference-best' style="text-align: center; color: #00aeef;">Best Conference Papers</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Conference' %}
        {% if item.award == 'Best Paper' %}
        
            {% for j in site.data.conferencepapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.Title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='conference-honorable' style="text-align: center; color: #00aeef;">Conference Papers - Honorable Mentions</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Conference' %}
        {% if item.award == 'Honorable Mention' %}
        
            {% for j in site.data.conferencepapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.Title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='conference-nominees' style="text-align: center; color: #00aeef;">Conference Papers - Nominees</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Conference' %}
        {% if item.award == 'Nominee' %}
        
            {% for j in site.data.conferencepapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.Title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='best-poster' style="text-align: center; color: #00aeef;">Best Poster</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Poster' %}
        {% if item.award == 'Best Poster' %}
        
            {% for j in site.data.posters %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='poster-honorable' style="text-align: center; color: #00aeef;">Posters - Honorable Mention</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Poster' %}
        {% if item.award == 'Honorable Mention' %}
        
            {% for j in site.data.posters %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='demo-best' style="text-align: center; color: #00aeef;">Best Demo</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Demo' %}
        {% if item.award == 'Best Demo' %}
        
            {% for j in site.data.demos %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='demo-honorable' style="text-align: center; color: #00aeef;">Demos - Honorable Mention</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Demo' %}
        {% if item.award == 'Honorable Mention' %}
        
            {% for j in site.data.demos %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='demo-people' style="text-align: center; color: #00aeef;">People's Choice Demo</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Demo' %}
        {% if item.award == 'People's Choice Demo' %}
        
            {% for j in site.data.demos %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='3dui-best' style="text-align: center; color: #00aeef;">3DUI Contest - Best 3DUI</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == '3DUI Contest' %}
        {% if item.award == 'Best 3DUI' %}
        
            {% for j in site.data.3dui %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>




