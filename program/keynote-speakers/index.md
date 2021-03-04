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
            <td><a href="#{{ keynote.id }}">Dr. {{ keynote.name }}</a></td>
            <td>{{ keynote.schedule }} - {{ keynote.timestart }} ({{ keynote.timezone }})</td>
        </tr>
        {% endfor %}
    </table>
</div>


{% for keynote in site.data.keynotes %}

<br />
<hr style="color: #00aeef">
<br />
<div id="{{ keynote.id }}">
    <center><strong><big>{{ keynote.name }}</big></strong></center>
    <center>{{ keynote.affiliation }}</center>
    <br />
    <center><img src="{{ keynote.photo }}" alt="Photo of {{ keynote.name }}" width="60%"></center>
    <br />

    <center><big><strong>{{ keynote.title }}</strong></big></center>
    <center><small>{{ keynote.schedule }}</small></center>

    <p>
        <strong>Abstract:</strong><br />
        {{ keynote.abstract }}
    </p>

    <p>
        <strong>Bio:</strong><br />
        {{ keynote.bio }}
    </p>

</div>

{% endfor %}

