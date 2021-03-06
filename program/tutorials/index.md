---
layout: ieeevr-default
title: "Tutorials"
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


<div>
    <table class="styled-table">

        <tr>
            <th>tutorials</th>
        </tr>
        {% for tutorial in site.data.tutorials %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ tutorial.id }}">{{ panel.tutorial }}</a></td>
        </tr>
        {% endfor %}
    </table>
</div>

<div>
    {% for panel in site.data.panels %}
    {% if panel.id == 'T1' %}
    <h2 id="{{ panel.id }}">Panel: {{ panel.title}}</h2>
    <p style="font-size: 0.8em;">{{ panel.day }}, {{panel.start}}, {{ panel.timezone }}</p>
    
    
    <h3 style="color: #00aeef;">Description</h3>
    <p>
        Research on the existence and nature of implicit bias has generated a significant amount of attention in psychology and other social sciences over the past few decades. Considerable scientific and policy interest in prejudice reduction and bias interventions date all the way back to such classic texts as Gordon Allport’s The Nature of Prejudice (1954), where intergroup contact theory as an approach to prejudice reduction was first introduced.  Thousands of hours and millions of dollars have been invested developing and implementing a wide variety of anti-discrimination and anti-bias training programs in different organizational and educational contexts. The efficacy of these efforts, and the conditions under which they are effective and for how long, continues to be an issue at the forefront of research on bias mitigation.
    </p>
      
    
    {% endif %}
    {% endfor %}
</div>



