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

</style>

<h1>Papers</h1>

<div>
    <table class="styled-table">
        <tr>
            <th>Monday, March 29</th>
        </tr>
        {% for session in site.data.sessions %}
            {% if session.schedule == 'Monday, March 29' %}
                <tr>
                    <td><a href="#{{ session.id }}">{{ session.name }}:{{ session.title }}</a></td>
                </tr>
            {% endif %}
        {% endfor %}
    </table>
</div>
<div>
    <table class="styled-table">
        <tr>
            <th>Tuesday, March 30</th>
        </tr>
        {% for session in site.data.sessions %}
            {% if session.schedule == 'Monday, March 29' %}
                <tr>
                    <td><a href="#{{ session.id }}">{{ session.name }}:{{ session.title }}</a></td>
                </tr>
            {% endif %}
        {% endfor %}
    </table>
</div>
<div>
    <table class="styled-table">
        <tr>
            <th>Wednesday, March 31</th>
        </tr>
        {% for session in site.data.sessions %}
            {% if session.schedule == 'Monday, March 29' %}
                <tr>
                    <td><a href="#{{ session.id }}">{{ session.name }}:{{ session.title }}</a></td>
                </tr>
            {% endif %}
        {% endfor %}
    </table>
</div>
<div>
    <table class="styled-table">
        <tr>
            <th>Thursday, April 1</th>
        </tr>
        {% for session in site.data.sessions %}
            {% if session.schedule == 'Monday, March 29' %}
                <tr>
                    <td><a href="#{{ session.id }}">{{ session.name }}:{{ session.title }}</a></td>
                </tr>
            {% endif %}
        {% endfor %}
    </table>
</div>

