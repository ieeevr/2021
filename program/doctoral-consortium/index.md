---
layout: ieeevr-default
title: "Doctoral Consortium"
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
        font-size: 0.9em;
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

<div>
    <table class="styled-table" style="font-size: 0.8em; ">
        <tr>
            <th>Schedule</th>
            <th></th>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">10:00 - 10:15 am</span></td>
            <td>
                Welcome + Ice Breaker
            </td>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">10:15 - 11:45 am</span></td>
            <td>
                <strong>Presentations 1 - 6 (8 min talk + 4 min questions)</strong><br/>
                Daniel Eckhoff - Dr. Gruchalla & Dr. Billinghurst<br/>
                Nermin Shaltout - Dr. Billinghurst and Dr. Quarles<br/>
                Shimmila Bhowmick - Dr. Froehlich and Dr. Correia<br/>
                Zhiming Hu - Dr. Robb and Dr. Potter<br/>
                Hannah Greber - Dr. Skarbez and Dr. Khadka<br/>
                Dilshani Kumarapeli - Dr. Stevenson Won and Dr. Skarbez<br/>
            </td>
        </tr>
        <tr>
            <td ><span style="color: #00aeef;">11:45 - 12:00 pm</span></td>
            <td>
                Break
            </td>
        </tr>
        <tr>
            <td ><span style="color: #00aeef;">12:00 - 1:30 pm</span></td>
            <td>
                <strong>Presentations 7 - 12 (8 min talk + 4 min questions)</strong><br/>
                Julia Belger - Dr. Stevenson Won and Dr. Suma Rosenberg<br/>
                Niklas Stein - Dr. Johnsen and Dr. Steed<br/>
                Alina Nikolaou - Dr. Potter and Dr. Johnsen<br/>
                Florian Mathis - Dr. Holz and Dr. Santos<br/>
                Eugene Kukshinov - Dr. Cutchin and Dr. Holz<br/>
                Nuno Cid Martins - Dr. Feiner and Dr. Khadka*
            </td>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">1:30 - 2:15 pm</span></td>
            <td>
                Break
            </td>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">2:15 - 4:15 pm</span></td>
            <td>
                <strong>Presentations 13 - 20 (8 min talk + 4 min questions)</strong><br/>
                Iris Willaert - Dr. Quarles and Dr. Gruchalla<br/>
                Valentin Vallageas - Dr. Suma Rosenberg and Dr. Peck<br/>
                Mohammed Safayet Arefin - Dr. Santos and Dr. Inami<br/>
                Feiyu Lu - Dr. Steed and Dr. Feiner<br/>
                Moloud Nasiri - Dr. Correia and Dr. Peck<br/>
                Amanda Zilla - Dr. Bowman and Dr. Cutchin<br/>
                Isayas Adhanom - Dr. Khadka and Dr. Bowman<br/>
                PS Berge - Dr. Inami and Dr. Robb
            </td>
        </tr>
        <tr>
            <td ><span style="color: #00aeef;">4:15 - 5:00 pm</span></td>
            <td>
                Mentoring Group 1 Breakout (45 min)
            </td>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">5:00 - 5:15 pm</span></td>
            <td>
                Break
            </td>
        </tr>
        <tr>
            <td ><span style="color: #00aeef;">5:15 - 6:00 pm</span></td>
            <td>
                Mentoring Group 2 Breakout (45 min)
            </td>
        </tr>
        <tr>
            <td ><span style="color: #00aeef;">6:00 - 6:05 pm</span></td>
            <td>
                Closing
            </td>
        </tr>
    </table>
</div>
    
    
</div>


<h2>Accepted Students</h2>

<div>
    <table class="styled-table" style="font-size: 0.8em; ">
        <tr>
            <th>Student</th>
            <th>Title</th>
            <th>Affiliation</th>
        </tr>
        {% for student in site.data.dc %}
        <tr>
            <td style="font-size: 0.8em;"><span style="color: #00aeef;">{{ student.author }}</span></td>
            <td>{{ student.title }}</td>
            <td>{{ student.affiliation }}</td>
        </tr>
        {% endfor %}
    </table>
</div>
