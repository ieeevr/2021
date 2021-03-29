---
layout: ieeevr-default
title: "Research Demos"
---

<style>
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
        border-bottom: 1px solid white;
        border-bottom-left-radius: 7px;
        border-bottom-right-radius: 7px;
        padding: .5rem 1rem;
    }

    .collapsible-content p {
        margin-bottom: 0;
    }
    
</style>


<div>
    <table class="styled-table">

        <tr>
            <th>Research Demos</th>
        </tr>
        {% for demo in site.data.demos %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ demo.id }}">{{ demo.title }}</a></td>
        </tr>
        {% endfor %}
    </table>
</div>

<div>
<!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'demos-all' %}
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
</div>

<div class="notice--info">
    <strong>Best of IEEE VR 2021</strong>
    <p>
        Please use this form to vote for the best poster, best demo, and best 3DUI contest submission.
    </p>
    <center>
        <p style="font-size: 20px;">
            <a href="https://cutt.ly/Mx0n5Zu" class="btn btn--primary" style="color: white;" target="_blank">Vote!</a>
        </p>
    </center>
</div>

<div>
    {% for demo in site.data.demos %}
    
    <h3 id="{{ demo.id }}">{{ demo.title }}</h3>
    <p><i>{{ demo.authors }}</i></p>
    
<p> <small><strong style="color: black;"> Booth: {{ demo.booth }} - {{ demo.hall }} </strong></small> <br> </p>    
    
    {% if demo.url %}
        <p>Teaser Video: <a href="{{ demo.url }}" target="_blank">Watch Now</a></p>
    {% endif %}
    {% if demo.abstract %}
    <div id="{{ demo.id }}" class="wrap-collabsible"> <input id="collapsible{{ demo.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ demo.id }}" class="lbl-toggle">Abstract</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <p>{{ demo.abstract }}</p>
            </div>
        </div>
    </div>
    {% endif %}
    {% endfor %}
</div>



