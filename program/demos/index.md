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

</style>


<div>
    <table class="styled-table">

        <tr>
            <th>Research Demos</th>
        </tr>
        {% for demo in site.data.demos %}
        <tr>
            <td><a href="#{{ demo.Id }}">{{ demo.Title }}</a></td>
        </tr>
        {% endfor %}
    </table>
</div>

<div>
    {% for demo in site.data.demos %}
    
    <h3 id="{{ demo.Id }}">{{ demo.Title }}</h3>
    <p>{{ demo.Abstract }}</p>
    <hr>
    {% endfor %}
</div>



