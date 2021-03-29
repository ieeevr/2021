---
layout: ieeevr-default
title: "Papers"
---

<style>
    .styled-table {
        border-collapse: collapse;
        margin: 25px 0;
        font-size: 0.9em;
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
        margin: 1rem 0;
    }

    .lbl-toggle {
        display: block;
        font-weight: bold;
        /* font-family: monospace; */
        font-size: 0.8rem;
        text-align: left;
        padding: 0rem;
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
        border-bottom: 1px solid white;
        border-bottom-left-radius: 7px;
        border-bottom-right-radius: 7px;
        padding: .5rem 1rem;
    }

    .collapsible-content p {
        margin-bottom: 0;
    }

</style>

<h1>Papers</h1>

<div>
    <table class="styled-table" style="font-size: 0.9em; ">
        <tr>
            <th>Monday, March 29, Lisbon WEST, UTC+1</th>
            <th></th>
        </tr>
        {% for session in site.data.sessions %}
        {% if session.day == 'Monday, March 29' %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ session.id }}">{{ session.name }}</a></td>
            <td>{{ session.starttime }} - {{ session.endtime }}</td>
        </tr>
        {% endif %}
        {% endfor %}
    </table>
</div>
<div>
    <table class="styled-table" style="font-size: 0.9em; ">
        <tr>
            <th>Tuesday, March 30, Lisbon WEST, UTC+1</th>
            <th></th>
        </tr>
        {% for session in site.data.sessions %}
        {% if session.day == 'Tuesday, March 30' %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ session.id }}">{{ session.name }}</a></td>
            <td>{{ session.starttime }} - {{ session.endtime }}</td>
        </tr>
        {% endif %}
        {% endfor %}
    </table>
</div>
<div>
    <table class="styled-table" style="font-size: 0.9em; ">
        <tr>
            <th>Wednesday, March 31, Lisbon WEST, UTC+1</th>
            <th></th>
        </tr>
        {% for session in site.data.sessions %}
        {% if session.day == 'Wednesday, March 31' %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ session.id }}">{{ session.name }}</a></td>
            <td>{{ session.starttime }} - {{ session.endtime }}</td>
        </tr>
        {% endif %}
        {% endfor %}
    </table>
</div>
<div>
    <table class="styled-table" style="font-size: 0.9em; ">
        <tr>
            <th>Thursday, April 1, Lisbon WEST, UTC+1</th>
            <th></th>
        </tr>
        {% for session in site.data.sessions %}
        {% if session.day == 'Thursday, April 1' %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ session.id }}">{{ session.name }}</a></td>
            <td>{{ session.starttime }} - {{ session.endtime }}</td>
        </tr>
        {% endif %}
        {% endfor %}
    </table>
</div>


<!-- 
INVITED MISSING
-->


{% for day in site.data.days %}
<div>
    {% for session in site.data.sessions %}
    {% if session.day == day.day' %}

    <h2 id="{{ session.id }}">Session: {{ session.name }}</h2>
    

    
    
    <p><strong>{{ session.day }}, {{ session.starttime }}, {{ session.timezone }}</strong></p>
    {% if session.sessionchair %}
    <p><small>Session Chair: <b style="font-family: 'Courier New', monospace; color: black;">{{ session.sessionchair }}</b></small></p>
    {% endif %}
    
        <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == session.id %}
    {% if event.location %}
    <div class="notice--info">
        <strong style="padding-bottom: 5px;">Take me to the event:</strong>
        <p>
            <strong style="color: black;">Virbela Location:</strong> {{ event.location }} (<a href="/2021/attend/virbela-instructions/#map">MAP</a>)

            {% if event.stream-url %}
            <br />
            {% if event.aindanaoaconteceu %}
            <strong style="color: black;">Watch video stream live:</strong> <a href="{{ event.stream-url }}" target="_blank">HERE</a>
            {% else %}
            <strong style="color: black;">Watch the recorded video stream:</strong> <a href="{{ event.stream-url }}" target="_blank">HERE</a>
            {% endif %}
            {% endif %}
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    

    {% for paper in site.data.papers %}
    {% if session.id == paper.session %}

    <h4 id="{{ paper.id }}">{{ paper.title }}</h4>
    <p><strong><small>{{ paper.type }}</small></strong></p>

    {% if paper.type == 'Journal' %}
    {% assign source = site.data.journalpapers %}
    {% endif %}

    {% if paper.type == 'Conference' %}
    {% assign source = site.data.conferencepapers %}
    {% endif %}

    {% if paper.type == 'Invited Journal' %}
    {% assign source = site.data.invitedjournalpapers %}
    {% endif %}

    {% for p in source %}
    {% if p.id == paper.id %}
    <p><i>{{ p.authors }}</i></p>
    <div id="{{ paper.id }}" class="wrap-collabsible"> <input id="collapsible{{ paper.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ paper.id }}" class="lbl-toggle">Abstract</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <p>{{ p.abstract }}</p>
            </div>
        </div>
    </div>
    {% endif %}
    {% endfor %}

    {% endif %}
    {% endfor %}

    {% endif %}
    {% endfor %}
</div>
{% endfor %}






<!--
<div id="S1">
    {% for session in site.data.sessions %}
    {% if session.id == 'S1' %}
    <h2>{{ session.name }}: {{ session.title }}</h2>
    {% endif %}
    {% endfor %}

    {% for paper in site.data.papers %}
    {% if paper.session == 'S1' %}

    <div>
        {% for demo in site.data.demos %}

        <h3 id="{{ paper.id }}">{{ paper.title }}</h3>
        <p><i>{{ paper.authors }}</i></p>
        <div id="{{ paper.id }}" class="wrap-collabsible"> <input id="collapsible{{ paper.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ paper.id }}" class="lbl-toggle">Abstract</label>
            <div class="collapsible-content">
                <div class="content-inner">
                    <p>{{ paper.abstract }}</p>
                </div>
            </div>
        </div>
        {% endfor %}
    </div>

    {% endif %}
    {% endfor %}
</div>
-->
