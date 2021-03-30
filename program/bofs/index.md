---
layout: ieeevr-default
title: "BoFs"
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
        
        width: 100%;
        margin-left: auto;
        margin-right: auto;
    }

    .styled-table thead tr {
        background-color: #00aeef;
        color: #ffffff;
        text-align: left;
    }

    .styled-table th,
    .styled-table td {
        padding: 12px 15px;
        width: 25%;
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
    
  /*div {
        text-align: justify;
        text-justify: inter-word;
        }*/
        
    
</style>

<div>
    
<h1>IEEE VR 2021 Birds of a Feather</h1>

<p> Shared interests bring VR 2021 attendees together! Registered attendees are invited to create their own social sessions using IEEE VR 2021 Virbela, Discord. 
    These are attendee-organized explorations or collaborations on topics impacting the field.
    We encourage attendees to consider any topic or idea, including purely social gatherings aimed at hanging out and chatting with other attendees. <br> </p> 
    <p> <strong>How?</strong> Register a BoF session using the google form on VR’s Discord (<b style="color: black">#bof</b>)! <br></p> 
    <p>We will collect them until Monday afternoon and create separate Discord channels for each. These will be published on Monday, also on the website, and in Virbela. Each organizer can use a Virbela room, the Discord channel, and will need to provide a zoom link for the video. As the organizer, you are responsible for ensuring a safe environment that follows the conference Code of Conduct. Please feel free to reach out to anyone on the conference committee if you need assistance, and please report any problematic behavior.</p>

</div>



<div>
    <table class="styled-table">

        {% for bof in site.data.bof %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ bof.id }}">{{ bof.name }}</a></td>
        </tr>
        {% endfor %}
    </table>
</div>






<div>
    {% for bof in site.data.bof %}
    
    <h2 id="{{ bof.id }}">BoF: {{ bof.name}}</h2>
    
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == bof.id %}
    {% if event.location %}
    <div class="notice--info">
        <strong style="padding-bottom: 5px;">Take me to the event:</strong>
        <p>
            {% if bof.id == 'BOFSocialX1' %}
            <strong style="color: black;">Virbela Location:</strong> VR Workshop Square -  Aveiro (<a href="/2021/attend/virbela-instructions/#map">MAP</a>)                     
            {% else %}
            <strong style="color: black;">Virbela Location:</strong> {{ event.location }} (<a href="/2021/attend/virbela-instructions/#map">MAP</a>)
            {% endif %}

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
    
    <p style="font-size: 0.8em;">{{ bof.session }}</p>
    
    <p> <strong> {{bof.chair}} </strong> <br> </p>
    <p> <strong style="color: black;"> Description: </strong> {{bof.description}}</p>
    
    
    {% endfor %}
</div>


