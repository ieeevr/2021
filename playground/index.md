---
layout: ieeevr-default
title: "playground"
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

</style>

<h1>IEEE VR 2021 Birds of a Feather</h1>

<p> Shared interests bring VR 2021 attendees together! Registered attendees are invited to create their own social sessions using IEEE VR 2021 Virbela, Discord. </p>
<p>These are attendee-organized explorations or collaborations on topics impacting the field.</p>
<p>We encourage attendees to consider any topic or idea, including purely social gatherings aimed at hanging out and chatting with other attendees. </p>
<p>How? Register a BoF session using the google form on VR’s Discord (#bof)</p>
<p>We will collect them until Monday afternoon and create separate Discord channels for each. These will be published on Monday, also on the website, and in Virbela. Each organizer can use a Virbela room, the Discord channel, and will need to provide a zoom link for the video. </p>
<p>As the organizer, you are responsible for ensuring a safe environment that follows the conference Code of Conduct. Please feel free to reach out to anyone on the conference committee if you need assistance, and please report any problematic behavior.</p>


<div>
    <table class="styled-table">

        {% for bof in site.data.bof %}
        <tr>
            <td style="font-size: 0.9em;">{{ bof.name }}</a></td>
        </tr>
        {% endfor %}
    </table>
</div>









