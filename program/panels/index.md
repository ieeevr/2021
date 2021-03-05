---
layout: ieeevr-default
title: "Panels"
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
            <th>Panels</th>
        </tr>
        {% for panel in site.data.panels %}
        <tr>
            <td style="font-size: 0.875em;"><a href="#{{ panel.id }}">{{ panel.name }}: {{ panel.title }}</a></td>
        </tr>
        {% endfor %}
    </table>
</div>

<div>
    {% for panel in site.data.panels %}
    {% if panel.id == 'P1' %}
    <h2 id="P1">{{ panel.name }}: {{ panel.title}}</h2>
    {% endif %}
    {% endfor %}




</div>
