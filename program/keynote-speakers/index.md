---
layout: ieeevr-default
title: "Keynote Speakers"
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

</style>

<h1>Keynote Speakers</h1>

<div>
    <table class="styled-table">

        <tr>
            <th></th>
            <th>Date</th>
        </tr>
        {% for keynote in site.data.keynotes %}
        <tr>
            <td><a href="#{{ keynote.id }}">{{ keynote.name }}</a></td>
            <td style="font-size: 0.875em;">{{ keynote.day }} - {{ keynote.start }} ({{ keynote.timezone }})</td>
        </tr>
        {% endfor %}
    </table>
</div>


{% for keynote in site.data.keynotes %}

<br />
<div id="{{ keynote.id }}">
    <center><strong><big>{{ keynote.name }}</big></strong></center>
    <center>{{ keynote.affiliation }}</center>
    <br />
    <center><img src="{{ keynote.photo }}" alt="Photo of {{ keynote.name }}" width="50%"></center>
    <br />

    <center><big><strong>{{ keynote.title }}</strong></big></center>
    <center><small>{{ keynote.day }} - {{ keynote.start }}, {{ keynote.timezone }}</small></center>
    {% if keynote.chair %}
    <center><small>Session Chair: <b style="font-family: 'Courier New', monospace; color: black;">{{ keynote.chair }}</b></small></center>
    
    {% endif %}
    
    
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == keynote.id %}
    {% if event.location %}
    <div id="{{ keynote.id }}-program" class="notice--info">
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
    
    
    <p>
        <strong>Abstract</strong><br />
        {{ keynote.abstract }}
    </p>

    <p>
        <strong>Bio</strong><br />
        {{ keynote.bio }}
    </p>
    
    <hr>

</div>

{% endfor %}

