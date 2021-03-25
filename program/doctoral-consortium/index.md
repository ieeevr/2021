---
layout: ieeevr-default
title: "Doctoral Consortium"
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

<h1>Doctoral Consortium</h1>
<div>
    <p>
        Here is the proposed schedule with mentor assignments. All of this time is Lisbon time (GMT+0). All presenters and mentors are encouraged to attend as much of the doctoral consortium as possible, however we understand that our different time zones may make attendance difficult at particular times. All talks will be recorded and available for later viewing. If a student and/or mentor are not available to meet during the scheduled mentoring sessions, they should set up a time to meet later that is convenient for them both.
    </p>
    <p>
        Mentors listed first next to a student will meet during the Mentor Group 1 Breakout session, and mentors listed second will meet with that student during the Mentor Group 2 Breakout session.
    </p>
</div>

<div>


</div>


<h2>Accepted Students</h2>

<div>
    <table class="styled-table" style="font-size: 0.9em; ">
        <tr>
            <th>Student</th>
            <th>Title</th>
        </tr>
        {% for student in site.data.dc %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ student.id }}">{{ student.author }}</a></td>
            <td>{{ student.title }}</td>
        </tr>
        {% endfor %}
    </table>
</div>
