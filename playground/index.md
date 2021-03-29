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


<div>
    <table class="styled-table">

        <tr>
            <th>Tutorials</th>
        </tr>
        {% for tutorial in site.data.tutorials %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ tutorial.id }}">{{ tutorial.title }}</a></td>
        </tr>
        {% endfor %}
    </table>
</div>

<!--
<table class="styled-table" style="font-size: 0.8em;">
            <tr>
                <th>BoF Session's Name</th>
                <th>Description</th>
                <th>Chair</th>
                <th>Time</th>
            </tr>
            {% for bof in site.data.bof %}
            <tr>
                <td style="font-size: 0.9em;">{{ bof.name }}</td>
                <td style="font-size: 0.9em;">{{ bof.description }}</td>
                <td style="font-size: 0.9em;">{{ bof.chair }}</td>
                <td style="font-size: 0.9em;">{{ bof.session }}</td>
                
            </tr>
            {% endfor %}
            
            </table>
            -->










