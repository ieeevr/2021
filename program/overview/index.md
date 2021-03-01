---
layout: ieeevr-default
title: "Program Overview"
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


    /*************************
 * GRID SCHEDULE LAYOUT
 *************************/
    @media screen and (min-width:700px) {
        .schedule {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0830] 1fr [time-0900] 1fr [time-0930] 1fr [time-1000] 1fr [time-1030] 1fr [time-1100] 1fr [time-1130] 1fr [time-1200] 1fr [time-1230] 1fr [time-1300] 1fr [time-1330] 1fr [time-1400] 1fr [time-1430] 1fr [time-1500] 1fr [time-1530] 1fr [time-1600] 1fr [time-1630] 1fr [time-1700] 1fr [time-1730] 1fr [time-1800] 1fr [time-1830] 1fr [time-1900] 1fr [time-1930] 1fr [time-2000] 1fr [time-2030] 1fr;
            /* Note 1:
      Use 24hr time for gridline names for simplicity

      Note 2: Use "auto" instead of "1fr" for a more compact schedule where height of a slot is not proportional to the session length. Implementing a "compact" shortcode attribute might make sense for this!
      Try 0.5fr for more compact equal rows. I don't quite understand how that works :)
      */

            grid-template-columns:
                [times] 4em [track-1-start] 1fr [track-1-end track-2-start] 1fr [track-2-end];
        }
    }
    
    @media screen and (min-width:700px) {
        .schedule-sat-27 {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0830] 1fr [time-0900] 1fr [time-0930] 1fr [time-1000] 1fr [time-1030] 1fr [time-1100] 1fr [time-1130] 1fr [time-1200] 1fr [time-1230] 1fr [time-1300] 1fr [time-1330] 1fr [time-1400] 1fr [time-1430] 1fr [time-1500] 1fr [time-1530] 1fr [time-1600] 1fr [time-1630] 1fr [time-1700] 1fr [time-1730] 1fr [time-1800] 1fr [time-1830] 1fr [time-1900] 1fr [time-1930] 1fr [time-2000] 1fr [time-2030] 1fr;
            /* Note 1:
      Use 24hr time for gridline names for simplicity

      Note 2: Use "auto" instead of "1fr" for a more compact schedule where height of a slot is not proportional to the session length. Implementing a "compact" shortcode attribute might make sense for this!
      Try 0.5fr for more compact equal rows. I don't quite understand how that works :)
      */

            grid-template-columns:
                [times] 4em
    [track-1-start] 1fr
    [track-1-end track-2-start] 1fr
    [track-2-end track-3-start] 1fr
    [track-3-end track-4-start] 1fr
    [track-4-end];
        }
    }

    .time-slot {
        grid-column: times;
        text-decoration: none;
        
    }

    .track-slot {
        display: none;
        /* hidden on small screens and browsers without grid support */
    }

    @supports(display:grid) {
        @media screen and (min-width:700px) {
            .track-slot {
                display: block;
                padding: 10px 5px 5px;
                position: sticky;
                top: 0;
                z-index: 1000;
                background-color: rgba(255, 255, 255, .9);
            }
        }
    }

    /* Small-screen & fallback styles */
    .session {
        margin-bottom: 1em;
    }

    @supports(display:grid) {
        @media screen and (min-width: 700px) {
            .session {
                margin: 0;
            }
        }
    }

    /*************************
 * VISUAL STYLES
 * Design-y stuff ot particularly important to the demo
 *************************/
    body {
        padding: 50px;
        max-width: 1100px;
        margin: 0 auto;
        line-height: 1.5;
    }

    .session {
        padding: .5em;
        border-radius: 2px;
        font-size: 14px;
        box-shadow:
            rgba(255, 255, 255, .6) 1px 1px 0,
            rgba(0, 0, 0, .3) 4px 4px 0;
    }

    .session-title,
    .session-time,
    .session-track,
    .session-presenter {
        display: block;
    }

    .session-title,
    .time-slot {
        margin: 0;
        font-size: 1em;
    }

    .session-title a {
        color: #fff;
        text-decoration-style: dotted;

        &:hover {
            font-style: italic;
        }

        &:focus {
            outline: 2px dotted rgba(255, 255, 255, .8);
        }
    }

    .track-slot,
    .time-slot {
        font-weight: bold;
        font-size: .75em;
    }

    .track-1 {
        background-color: #1259B2;
        color: #fff;
    }

    .track-2 {
        background-color: #687f00;
        color: #fff;
    }

    .track-3 {
        background-color: #544D69;
        color: #fff;
    }

    .track-4 {
        background-color: #c35500;
        color: #fff;
    }

    .track-all {
        display: flex;
        justify-content: center;
        align-items: center;
        background: #ccc;
        color: #000;
        box-shadow: none;
    }

    .track-event-all {
        background-color: #00aeef;
        color: #fff;
    }

    .track-break {
        background-color: #ddf6ff;
        color: #464646;
    }

    .track-papers {
        background-color: rgb(52, 199, 89);
        color: #fff;
    }

    .track-posters-demos {
        background-color: rgb(255, 149, 0);
        color: #fff;
    }

    .track-event {
        background-color: rgb(90, 200, 250);
        color: #fff;
    }

    .track-panel {
        background-color: rgb(0, 122, 255);
        color: #fff;
    }

    .track-keynote {
        background-color: rgb(255, 45, 85);
        color: #fff;
    }

    .text {
        max-width: 750px;
        font-size: 18px;
        margin: 0 auto 50px;
    }

    .meta {
        color: #555;
        font-style: italic;
    }

    .meta a {
        color: #555;
    }

    hr {
        margin: 40px 0;
    }

</style>

<div>
    <h1>Program Overview</h1>


    <h2>Panel Sessions</h2>

    <table class="styled-table">

        <tr>
            <th>Session</th>
            <th>Topic Area</th>
        </tr>

        <tr>
            <td>1</td>
            <td>Ethics and Privacy in Mixed Reality</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Ethics and Privacy in Mixed Reality</td>
        </tr>

    </table>



    <h2>Paper Sessions</h2>

    <table class="styled-table">

        <tr>
            <th>Session</th>
            <th>Topic Area</th>
        </tr>

        <tr>
            <td>1</td>
            <td>Ethics and Privacy in Mixed Reality</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Ethics and Privacy in Mixed Reality</td>
        </tr>

    </table>


    <h2>Saturday, March 27</h2>
    <div class="schedule-sat-27" aria-labelledby="schedule-heading">

        <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon (WEST)</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;">Track 3</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;">Track 4</span>

        <p class="time-slot" style="grid-row: time-0830; text-decoration: none;">8:30</p>

        <div class="session session-1 track-event-all" style="grid-column: track-1-start / track-2-end; grid-row: time-0830 / time-1000;">
            <h3 class="session-title"><a href="#">Opening</a></h3>
            <span class="session-time">8:30 - 10:00</span>
        </div>
    
    </div>
    
    
    
    
    
    
    
    <h2>Sunday, March 28</h2>

    <!-- MONDAY, MARCH 29 -->
    <h2>Monday, March 29</h2>
    <div class="schedule" aria-labelledby="schedule-heading">

        <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon (WEST)</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>

        <p class="time-slot" style="grid-row: time-0830; text-decoration: none;">8:30</p>

        <div class="session session-1 track-event-all" style="grid-column: track-1-start / track-2-end; grid-row: time-0830 / time-1000;">
            <h3 class="session-title"><a href="#">Opening</a></h3>
            <span class="session-time">8:30 - 10:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1000;">10:00</p>

        <div class="session session-2 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1000 / time-1030;">
            <h3 class="session-title">Break</h3>
        </div>

        <p class="time-slot" style="grid-row: time-1030;">10:30</p>

        <div class="session session-3 track-keynote" style="grid-column: track-1-start / track-2-end; grid-row: time-1030 / time-1130;">
            <h3 class="session-title">Keynote</h3>
            <span class="session-time">10:30 - 11:30</span>
        </div>

        <p class="time-slot" style="grid-row: time-1130;">11:30</p>

        <div class="session session-4 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1130 / time-1200;">
            <h3 class="session-title">Break</h3>
        </div>

        <p class="time-slot" style="grid-row: time-1200;">12:00</p>

        <div class="session session-5 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1200 / time-1300;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">12:00 - 13:00</span>
        </div>

        <div class="session session-6 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1200 / time-1300;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">12:00 - 13:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1300;">13:00</p>
        <div class="session session-7 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1300 / time-1400;">
            <h3 class="session-title">Lunch</h3>
        </div>

        <p class="time-slot" style="grid-row: time-1400;">14:00</p>

        <div class="session session-8 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1500;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">14:00 - 15:00</span>
        </div>

        <div class="session session-9 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1500;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">14:00 - 15:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1500;">15:00</p>
        <div class="session session-10 track-posters-demos" style="grid-column: track-1-start / track-2-end; grid-row: time-1500 / time-1630;">
            <h3 class="session-title">Posters and Demos</h3>
            <span class="session-time">15:00 - 16:30</span>
        </div>


        <p class="time-slot" style="grid-row: time-1630;">16:30</p>

        <div class="session session-5 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1630 / time-1730;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">16:30 - 17:30</span>
        </div>

        <div class="session session-6 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1630 / time-1730;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">16:30 - 17:30</span>
        </div>

        <p class="time-slot" style="grid-row: time-1730;">17:30</p>
        <div class="session session-10 track-event-all" style="grid-column: track-1-start / track-2-end; grid-row: time-1730 / time-1900;">
            <h3 class="session-title">Welcome Reception</h3>
            <span class="session-time">17:30 - 19:00</span>
        </div>

    </div>

    <!-- TUESDAY, MARCH 30 -->
    <h2>Tuesday, March 30</h2>
    <div class="schedule" aria-labelledby="schedule-heading">

        <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon (WEST)</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>

        <p class="time-slot" style="grid-row: time-0830;">8:30</p>

        <div class="session session-1 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0930;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">8:30 - 9:30</span>
        </div>

        <div class="session session-2 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0930;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">8:30 - 9:30</span>
        </div>

        <p class="time-slot" style="grid-row: time-0930;">9:30</p>
        <div class="session session-3 track-posters-demos" style="grid-column: track-1-start / track-2-end; grid-row: time-0930 / time-1100;">
            <h3 class="session-title">Posters and Demos</h3>
            <span class="session-time">9:30 - 11:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1100;">11:00</p>

        <div class="session session-4 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1100 / time-1200;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">8:30 - 9:30</span>
        </div>

        <div class="session session-5 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1100 / time-1200;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">11:00 - 12:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1200;">12:00</p>
        <div class="session session-6 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1200 / time-1300;">
            <h3 class="session-title">Lunch</h3>
        </div>

        <p class="time-slot" style="grid-row: time-1300;">13:00</p>

        <div class="session session-7 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1300 / time-1400;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">13:00 - 14:00</span>
        </div>

        <div class="session session-8 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1300 / time-1400;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">13:00 - 14:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1400;">14:00</p>

        <div class="session session-9 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1400 / time-1430;">
            <h3 class="session-title">Break</h3>
        </div>

        <p class="time-slot" style="grid-row: time-1430;">14:30</p>

        <div class="session session-10 track-keynote" style="grid-column: track-1-start / track-2-end; grid-row: time-1430 / time-1530;">
            <h3 class="session-title">Keynote</h3>
            <span class="session-time">14:30 - 15:30</span>
        </div>

        <p class="time-slot" style="grid-row: time-1530;">15:30</p>

        <div class="session session-11 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1530 / time-1600;">
            <h3 class="session-title">Break</h3>
        </div>

        <p class="time-slot" style="grid-row: time-1600;">16:00</p>
        <div class="session session-12 track-event" style="grid-column: track-1-start / track-2-end; grid-row: time-1600 / time-1700;">
            <h3 class="session-title">BOF/Social</h3>
            <span class="session-time">16:00 - 17:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1700;">17:00</p>

        <div class="session session-13 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1700 / time-1800;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">17:00 - 18:00</span>
        </div>

        <div class="session session-14 track-panel" style="grid-column: track-2-start / track-2-end; grid-row: time-1700 / time-1800;">
            <h3 class="session-title">Panel</h3>
            <span class="session-time">17:00 - 18:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1800;">18:00</p>
        <div class="session session-15 track-event" style="grid-column: track-1-start / track-2-end; grid-row: time-1800 / time-1900;">
            <h3 class="session-title">Mixer</h3>
            <span class="session-time">18:00 - 19:00</span>
        </div>

    </div>

    <!-- WEDNESDAY, MARCH 31 -->
    <h2>Wednesday, March 31</h2>
    <div class="schedule" aria-labelledby="schedule-heading">

        <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon (WEST)</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>

        <p class="time-slot" style="grid-row: time-0830;">8:30</p>

        <div class="session session-1 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0930;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">8:30 - 9:30</span>
        </div>

        <div class="session session-2 track-panel" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0930;">
            <h3 class="session-title">Panel</h3>
            <span class="session-time">8:30 - 9:30</span>
        </div>

        <p class="time-slot" style="grid-row: time-0930;">09:30</p>
        <div class="session session-3 track-event" style="grid-column: track-1-start / track-2-end; grid-row: time-0930 / time-1030;">
            <h3 class="session-title">BOF/Social</h3>
            <span class="session-time">9:30 - 10:30</span>
        </div>

        <p class="time-slot" style="grid-row: time-1030;">10:30</p>

        <div class="session session-4 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1030 / time-1100;">
            <h3 class="session-title">Break</h3>
        </div>

        <p class="time-slot" style="grid-row: time-1100;">11:00</p>

        <div class="session session-5 track-keynote" style="grid-column: track-1-start / track-2-end; grid-row: time-1100 / time-1200;">
            <h3 class="session-title">Keynote</h3>
            <span class="session-time">11:00 - 12:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1200;">12:00</p>
        <div class="session session-6 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1200 / time-1300;">
            <h3 class="session-title">Lunch</h3>
        </div>

        <p class="time-slot" style="grid-row: time-1300;">13:00</p>

        <div class="session session-7 track-event" style="grid-column: track-1-start / track-1-end; grid-row: time-1300 / time-1400;">
            <h3 class="session-title">Mixer</h3>
            <span class="session-time">13:00 - 14:00</span>
        </div>

        <div class="session session-8 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1300 / time-1400;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">13:00 - 14:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1400;">14:00</p>
        <div class="session session-9 track-posters-demos" style="grid-column: track-1-start / track-2-end; grid-row: time-1400 / time-1530;">
            <h3 class="session-title">Posters and Demos</h3>
            <span class="session-time">14:00 - 15:30</span>
        </div>

        <p class="time-slot" style="grid-row: time-1530;">15:30</p>

        <div class="session session-10 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1530 / time-1630;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">15:30 - 16:30</span>
        </div>

        <div class="session session-11 track-panel" style="grid-column: track-2-start / track-2-end; grid-row: time-1530 / time-1630;">
            <h3 class="session-title">Panel</h3>
            <span class="session-time">15:30 - 16:30</span>
        </div>

        <p class="time-slot" style="grid-row: time-1630;">16:30</p>

        <div class="session session-12 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1630 / time-1700;">
            <h3 class="session-title">Break</h3>
        </div>

        <p class="time-slot" style="grid-row: time-1700;">17:00</p>

        <div class="session session-13 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1700 / time-1800;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">17:00 - 18:00</span>
        </div>

        <div class="session session-14 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1700 / time-1800;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">17:00 - 18:00</span>
        </div>

        <p class="time-slot" style="grid-row: time-1800;">18:00</p>
        <div class="session session-15 track-event" style="grid-column: track-1-start / track-2-end; grid-row: time-1800 / time-1900;">
            <h3 class="session-title">Mixer</h3>
            <span class="session-time">18:00 - 19:00</span>
        </div>

    </div>


    <!-- THUSDAY, APRIL 1 -->
    <h2>Thursday, April 1</h2>
    <div class="schedule" aria-labelledby="schedule-heading">

        <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon (WEST)</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
        <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>

        <p class="time-slot" style="grid-row: time-0830;">8:30</p>

        <div class="session session-1 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0930;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">8:30 - 9:30</span>
        </div>

        <div class="session session-2 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0930;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">8:30 - 9:30</span>
        </div>

        <p class="time-slot" style="grid-row: time-0930;">09:30</p>
        <div class="session session-3 track-event" style="grid-column: track-1-start / track-2-end; grid-row: time-0930 / time-1030;">
            <h3 class="session-title">BOF/Social</h3>
            <span class="session-time">9:30 - 10:30</span>
        </div>
        
        <p class="time-slot" style="grid-row: time-1030;">10:30</p>
        <div class="session session-4 track-posters-demos" style="grid-column: track-1-start / track-2-end; grid-row: time-1030 / time-1200;">
            <h3 class="session-title">Posters and Demos</h3>
            <span class="session-time">10:30 - 12:00</span>
        </div>
        
        <p class="time-slot" style="grid-row: time-1200;">12:00</p>

        <div class="session session-5 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1200 / time-1300;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">12:00 - 13:00</span>
        </div>

        <div class="session session-5 track-panel" style="grid-column: track-2-start / track-2-end; grid-row: time-1200 / time-1300;">
            <h3 class="session-title">Panel</h3>
            <span class="session-time">12:00 - 13:00</span>
        </div>
        
        <p class="time-slot" style="grid-row: time-1300;">13:00</p>
        <div class="session session-7 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1300 / time-1400;">
            <h3 class="session-title">Lunch</h3>
        </div>
        
        <p class="time-slot" style="grid-row: time-1400;">14:00</p>

        <div class="session session-8 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1500;">
            <h3 class="session-title">Paper Session</h3>
            <span class="session-time">14:00 - 15:00</span>
        </div>

        <div class="session session-9 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1500;">
            <h3 class="session-title">Papers</h3>
            <span class="session-time">14:00 - 15:00</span>
        </div>
        
        <p class="time-slot" style="grid-row: time-1500;">15:00</p>

        <div class="session session-10 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1500 / time-1530;">
            <h3 class="session-title">Break</h3>
        </div>
        
        <p class="time-slot" style="grid-row: time-1530;">15:30</p>

        <div class="session session-11 track-keynote" style="grid-column: track-1-start / track-2-end; grid-row: time-1530 / time-1630;">
            <h3 class="session-title">Keynote</h3>
            <span class="session-time">15:30 - 16:30</span>
        </div>
        
        <p class="time-slot" style="grid-row: time-1630;">16:30</p>

        <div class="session session-2 track-event-all" style="grid-column: track-1-start / track-2-end; grid-row: time-1630 / time-1800;">
            <h3 class="session-title"><a href="#">Closing</a></h3>
            <span class="session-time">6:30 - 18:00</span>
        </div>
        
    </div>
    
    
    
    <h2>Friday, April 2</h2>
    
    <!--
<div class="schedule" aria-labelledby="schedule-heading">
  
  <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
  <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>
  <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;">Track 3</span>
  <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;">Track 4</span>
  
  <h2 class="time-slot" style="grid-row: time-0800;">8:00am</h2>

  <div class="session session-1 track-1" style="grid-column: track-1; grid-row: time-0800 / time-0900;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">8:00 - 9:00</span>
    <span class="session-track">Track: 1</span>
    <span class="session-presenter">Presenter</span>
  </div>
  
  <div class="session session-2 track-2" style="grid-column: track-2; grid-row: time-0800 / time-0830;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">8:00 - 8:30</span>
    <span class="session-track">Track: 2</span>
    <span class="session-presenter">Presenter</span>
  </div>  
  
  <div class="session session-3 track-3" style="grid-column: track-3; grid-row: time-0800 / time-0830;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">8:00 - 8:30</span>
    <span class="session-track">Track: 3</span>
    <span class="session-presenter">Presenter</span>
  </div>
  
  <div class="session session-4 track-4" style="grid-column: track-4; grid-row: time-0800 / time-1000;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">8:00 - 10:00</span>
    <span class="session-track">Track: 2</span>
    <span class="session-presenter">Presenter</span>
  </div>
  
  <h2 class="time-slot" style="grid-row: time-0830;">8:30am</h2>
  
  <div class="session session-5 track-3" style="grid-column: track-3; grid-row: time-0830 / time-1000;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">8:30 - 10:00</span>
    <span class="session-track">Track: 1</span>
    <span class="session-presenter">Presenter</span>
  </div>
  
  <h2 class="time-slot" style="grid-row: time-0900;">9:00am</h2>
  
  <div class="session session-6 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-0900 / time-1000;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">9:00 - 10:00</span>
    <span class="session-track">Track: 1 & 2</span>
    <span class="session-presenter">Presenter</span>
  </div>
  
  <h2 class="time-slot" style="grid-row: time-1000;">10:00am</h2>
  
  <div class="session session-7 track-all" style="grid-column: track-1-start / track-4-end; grid-row: time-1000 / time-1030;">
    <h3 class="session-title">Take a break!</h3>
  </div>
  
  <h2 class="time-slot" style="grid-row: time-1030;">10:30am</h2>
  
  <div class="session session-8 track-1" style="grid-column: track-1; grid-row: time-1030 / time-1130;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">10:30 - 11:30</span>
    <span class="session-track">Track: 1</span>
    <span class="session-presenter">Presenter</span>
  </div>
  
  <div class="session session-9 track-2" style="grid-column: track-2-start / track-3-end; grid-row: time-1030 / time-1100;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">10:30 - 11:00</span>
    <span class="session-track">Track: 2 & 3</span>
    <span class="session-presenter">Presenter</span>
  </div>
  
  <div class="session session-10 track-4" style="grid-column: track-4; grid-row: time-1030 / time-1100;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">10:30 - 11:00</span>
    <span class="session-track">Track: 4</span>
    <span class="session-presenter">Presenter</span>
  </div>
  
  <h2 class="time-slot" style="grid-row: time-1100;">11:00am</h2>
  
  <div class="session session-11 track-2" style="grid-column: track-2; grid-row: time-1100 / time-1200;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">11:00 - 12:00</span>
    <span class="session-track">Track: 2</span>
    <span class="session-presenter">Presenter</span>
  </div>
  
  <div class="session session-11 track-3" style="grid-column: track-3; grid-row: time-1100 / time-1200;">
    <h3 class="session-title"><a href="#">Talk Title</a></h3>
    <span class="session-time">11:00 - 12:00</span>
    <span class="session-track">Track: 3</span>
    <span class="session-presenter">Presenter</span>
  </div>
  
</div>
-->





</div>
