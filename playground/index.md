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
 * GRID SCHEDULE LAYOUT from there: https://css-tricks.com/building-a-conference-schedule-with-css-grid/
 *************************/
    @media screen and (min-width:700px) {
        .schedule {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0830] 0.1fr [time-0900] 0.1fr [time-0930] 0.1fr [time-1000] 0.1fr [time-1030] 0.1fr [time-1100] 0.1fr [time-1130] 0.1fr [time-1200] 0.1fr [time-1230] 0.1fr [time-1300] 0.1fr [time-1330] 0.1fr [time-1400] 0.1fr [time-1430] 0.1fr [time-1500] 0.1fr [time-1530] 0.1fr [time-1600] 0.1fr [time-1630] 0.1fr [time-1700] 0.1fr [time-1730] 0.1fr [time-1800] 0.1fr [time-1830] 0.1fr [time-1900] 0.1fr;
            /* Note 1:
      Use 24hr time for gridline names for simplicity

      Note 2: Use "auto" instead of "0.5fr" for a more compact schedule where height of a slot is not proportional to the session length. Implementing a "compact" shortcode attribute might make sense for this!
      Try 0.5fr for more compact equal rows. I don't quite understand how that works :)
      */

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end];
        }

        .schedule-sat-27 {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0900] 5px [time-0930] 5px [time-1000] 5px [time-1030] 5px [time-1100] 5px [time-1130] 5px [time-1200] 5px [time-1230] 5px [time-1300] 5px [time-1330] 5px [time-1400] 5px [time-1430] 5px [time-1500] 5px [time-1530] 5px [time-1600] 5px [time-1630] 5px [time-1700] 5px [time-1730] 5px [time-1800] 5px [time-1830] 5px [time-1900] 5px;

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end track-4-start] 0.5fr [track-4-end];
        }

        .schedule-sun-28 {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0900] 5px [time-0930] 5px [time-1000] 5px [time-1030] 5px [time-1100] 5px [time-1130] 5px [time-1200] 5px [time-1230] 5px [time-1300] 5px [time-1330] 5px [time-1400] 5px [time-1430] 5px [time-1500] 5px [time-1530] 5px [time-1600] 5px [time-1630] 5px [time-1700] 5px [time-1730] 5px [time-1800] 5px [time-1830] 5px [time-1900] 5px [time-1930] 5px [time-2000] 5px [time-2030] 5px;

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end];
        }

        .schedule-fri-2 {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0900] 5px [time-0930] 5px [time-1000] 5px [time-1030] 5px [time-1100] 5px [time-1130] 5px [time-1200] 5px [time-1230] 5px [time-1300] 5px [time-1330] 5px [time-1400] 5px [time-1430] 5px [time-1500] 5px [time-1530] 10px [time-1600] 5px [time-1630] 5px [time-1700] 5px [time-1730] 5px [time-1800] 5px [time-1830] 5px [time-1900] 5px [time-1930] 5px [time-2000] 5px [time-2030] 5px;

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end];
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
 ************************
    body {
        padding: 50px;
        max-width: 1100px;
        margin: 0 auto;
        line-height: 1.5;
    }
    */

    .session {
        padding: .5em;
        border-radius: 5px;
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

    .track-teal {
        background-color: #00aeef;
        color: #fff;
    }

    .track-break {
        background-color: #ddf6ff;
        color: #464646;
    }

    .track-green {
        background-color: rgb(52, 199, 89);
        color: #fff;
    }

    .track-orange {
        background-color: rgb(255, 149, 0);
        color: #fff;
    }
    
    .track-purple {
        background-color: rgb(175, 82, 222);
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


    /* Collapsible */
    input[type='checkbox'] {
        display: none;
    }

    .wrap-collabsible {
        margin: 1.2rem 0;
    }

    .lbl-toggle {
        display: block;
        font-weight: bold;
        /* font-family: monospace; */
        font-size: 1rem;
        text-align: left;
        padding: 0.5rem;
        color: #ffffff;
        background: #00aeef;
        cursor: pointer;
        border-radius: 7px;
        transition: all 0.25s ease-out;
    }

    .lbl-toggle:hover {
        color: #FFF;
    }

    .lbl-toggle::before {
        content: ' ';
        display: inline-block;
        border-top: 5px solid transparent;
        border-bottom: 5px solid transparent;
        border-left: 5px solid currentColor;
        vertical-align: middle;
        margin-right: .7rem;
        transform: translateY(-2px);
        transition: transform .2s ease-out;
    }

    .toggle:checked+.lbl-toggle::before {
        transform: rotate(90deg) translateX(-3px);
    }

    .collapsible-content {
        max-height: 0px;
        overflow: hidden;
        transition: max-height .25s ease-in-out;
    }

    .toggle:checked+.lbl-toggle+.collapsible-content {
        max-height: 1500px;
    }

    .toggle:checked+.lbl-toggle {
        border-bottom-right-radius: 0;
        border-bottom-left-radius: 0;
    }

    .collapsible-content .content-inner {
        background: white;
        /* rgba(0, 105, 255, .2);*/
        border-bottom: 1px solid rgba(0, 105, 255, .45);
        border-bottom-left-radius: 7px;
        border-bottom-right-radius: 7px;
        padding: .5rem 1rem;
    }

    .collapsible-content p {
        margin-bottom: 0;
    }

</style>


<h1>Program Overview</h1>

<div>
    <div class="wrap-collabsible"> <input id="collapsible1" class="toggle" type="checkbox" checked> <label for="collapsible1" class="lbl-toggle">Saturday, March 27</label>
        <div class="collapsible-content">
            <div class="content-inner">

                <div class="schedule-sat-27" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon WET, UTC</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;">Track 3</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;">Track 4</span>

                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>

                    <div class="session session-1 track-teal" style="grid-column: track-1-start / track-1-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="#">Tutorial: Interactive Storytelling for VR</a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                    </div>

                    <div class="session session-2 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#SIVE">Workshop: Sonic Interactions in Virtual Environments (SIVE) </a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                    </div>

                    <div class="session session-3 track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#EXR">Workshop: Ethics in VR (EXR)</a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                    </div>

                    <div class="session session-4 track-orange" style="grid-column: track-4-start / track-4-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="#">Doctoral Consortium</a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                    </div>


                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>

                    <div class="session session-5 track-teal" style="grid-column: track-1-start / track-1-end; grid-row: time-1300 / time-1600;">
                        <h3 class="session-title"><a href="#">Tutorial: Web-Based VR Development and Instruction using Babylon.js</a></h3>
                        <span class="session-time">13:00 - 16:00</span>
                    </div>

                    <div class="session session-6 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1300 / time-1700;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#NIDIT">Workshop: Novel Input Devices and Interaction Techniques (NIDIT)</a></h3>
                        <span class="session-time">13:00 - 17:00</span>
                    </div>

                    <div class="session session-7 track-orange" style="grid-column: track-4-start / track-4-end; grid-row: time-1300 / time-1600;">
                        <h3 class="session-title"><a href="#">Doctoral Consortium</a></h3>
                        <span class="session-time">13:00 - 16:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>
                    <div class="session session-8 track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-1530 / time-2100;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#DISCE">Workshop: Distributed Interactive Systems for Collaborative Experiences (DISCE) </a></h3>
                        <span class="session-time">15:00 - 21:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1700;">15:30</p>
                    <div class="session session-9 track-teal" style="grid-column: track-1-start / track-1-end; grid-row: time-1700 / time-2100;">
                        <h3 class="session-title"><a href="#">Tutorial: OpenAR: Combining the Virtual and Real?</a></h3>
                        <span class="session-time">15:30 - 21:00</span>
                    </div>
                    <div class="session session-10 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1700 / time-2100;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#VHCIE2021">Workshop: Virtual Humans and Crowds for Immersive Environments (VHCIE 2021)</a></h3>
                        <span class="session-time">17:00 - 21:00</span>
                    </div>
                    <div class="session session-11 track-orange" style="grid-column: track-4-start / track-4-end; grid-row: time-1700 / time-2100;">
                        <h3 class="session-title"><a href="#">Doctoral Consortium</a></h3>
                        <span class="session-time">17:00 - 21:00</span>
                    </div>

                </div>

            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible2" class="toggle" type="checkbox" checked> <label for="collapsible2" class="lbl-toggle">Sunday, March 28</label>
        <div class="collapsible-content">
            <div class="content-inner">

                <div class="schedule-sun-28" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon WEST UTC+1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;">Track 3</span>

                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>

                    <div class="session session-1 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#ANIVAE">Workshop: Animation in Virtual and Augmented Environments (ANIVAE)</a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <div class="session session-2 track-teal" style="grid-column: track-1-start / track-1-end; grid-row: time-1300 / time-1600;">
                        <h3 class="session-title"><a href="#">Tutorial: The Replication Crisis in Empirical Science: Implications for Human Subject Research in MR</a></h3>
                        <span class="session-time">13:00 - 16:00</span>
                    </div>
                    <div class="session session-3 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1300 / time-1600;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#PrXR">Workshop: PrXR: Towards a roadmap for privacy and security research for mixed reality applications</a></h3>
                        <span class="session-time">13:00 - 16:00</span>
                    </div>
                    <div class="session session-4 track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-1300 / time-1600;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#TrainingXR">Workshop: 3D Content Creation for Simulated Training in eXtended Reality (TrainingXR) - 1</a></h3>
                        <span class="session-time">13:00 - 16:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>
                    <div class="session session-5 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1700 / time-2100;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#SeatedVR">Workshop: Seated Virtual Reality & Embodiment (SeatedVR) </a></h3>
                        <span class="session-time">17:00 - 21:00</span>
                    </div>
                    <div class="session session-6 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1700 / time-2100;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#WISP">Workshop: Workshop on Immersive Sickness Prevention (WISP)</a></h3>
                        <span class="session-time">17:00 - 21:00</span>
                    </div>
                    <div class="session session-7 track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-1700 / time-2100;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#TrainingXR">Workshop: 3D Content Creation for Simulated Training in eXtended Reality (TrainingXR) - 2</a></h3>
                        <span class="session-time">17:00 - 21:00</span>
                    </div>
                </div>

            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible3" class="toggle" type="checkbox" checked> <label for="collapsible3" class="lbl-toggle">Monday, March 29</label>
        <div class="collapsible-content">
            <div class="content-inner">

                <div class="schedule" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon WEST UTC+1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 3</span>

                    <p class="time-slot" style="grid-row: time-0830; text-decoration: none;">8:30</p>

                    <div class="session session-1 track-teal" style="grid-column: track-1-start / track-2-end; grid-row: time-0830 / time-1000;">
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

                    <div class="session session-5 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">12:00 - 13:00</span>
                    </div>

                    <div class="session session-6 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">12:00 - 13:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <div class="session session-7 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Lunch</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>

                    <div class="session session-8 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>

                    <div class="session session-9 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>
                    <div class="session session-10 track-orange" style="grid-column: track-1-start / track-2-end; grid-row: time-1500 / time-1630;">
                        <h3 class="session-title">Posters and Demos</h3>
                        <span class="session-time">15:00 - 16:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>
                    <div class="session session-ex track-purple" style="grid-column: track-1-start / track-1-end; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title"><a href="/2021/contribute/exhibitors/">Exhibition Hours</a></h3>
                        <span class="session-time">16:00 - 17:30</span>
                    </div>
                    
                    
                    <p class="time-slot" style="grid-row: time-1630;">16:30</p>

                    <div class="session session-5 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1630 / time-1730;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">16:30 - 17:30</span>
                    </div>

                    <div class="session session-6 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1630 / time-1730;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">16:30 - 17:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1730;">17:30</p>
                    <div class="session session-10 track-teal" style="grid-column: track-1-start / track-2-end; grid-row: time-1730 / time-1900;">
                        <h3 class="session-title">Welcome Reception</h3>
                        <span class="session-time">17:30 - 19:00</span>
                    </div>

                </div>

            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible7" class="toggle" type="checkbox" checked> <label for="collapsible7" class="lbl-toggle">Tuesday, March 30</label>
        <div class="collapsible-content">
            <div class="content-inner">

                <div class="schedule" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon WEST UTC+1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>

                    <p class="time-slot" style="grid-row: time-0830;">8:30</p>

                    <div class="session session-1 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">8:30 - 9:30</span>
                    </div>

                    <div class="session session-2 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">8:30 - 9:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-0930;">9:30</p>
                    <div class="session session-3 track-orange" style="grid-column: track-1-start / track-2-end; grid-row: time-0930 / time-1100;">
                        <h3 class="session-title">Posters and Demos</h3>
                        <span class="session-time">9:30 - 11:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>

                    <div class="session session-4 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">11:00 - 12:00</span>
                    </div>

                    <div class="session session-5 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">11:00 - 12:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>
                    <div class="session session-6 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Lunch</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>

                    <div class="session session-7 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">13:00 - 14:00</span>
                    </div>

                    <div class="session session-8 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1300 / time-1400;">
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

                    <div class="session session-13 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1700 / time-1800;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">17:00 - 18:00</span>
                    </div>

                    <div class="session session-14 track-panel" style="grid-column: track-2-start / track-2-end; grid-row: time-1700 / time-1830;">
                        <h3 class="session-title"><a href="/2021/program/panels/#P1">Panel: Opportunities and Challenges in Harnessing VR Technology for Bias Mitigation</a></h3>
                        <span class="session-time">17:00 - 18:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>
                    <div class="session session-15 track-event" style="grid-column: track-1-start / track-1-end; grid-row: time-1800 / time-1900;">
                        <h3 class="session-title">Mixer</h3>
                        <span class="session-time">18:00 - 19:00</span>
                    </div>

                </div>

            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible4" class="toggle" type="checkbox" checked> <label for="collapsible4" class="lbl-toggle">Wednesday, March 31</label>
        <div class="collapsible-content">
            <div class="content-inner">

                <div class="schedule" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon WEST UTC+1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>

                    <p class="time-slot" style="grid-row: time-0830;">8:30</p>

                    <div class="session session-1 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">8:30 - 9:30</span>
                    </div>

                    <div class="session session-2 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Paper Session</h3>
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

                    <div class="session session-8 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">13:00 - 14:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>
                    <div class="session session-9 track-orange" style="grid-column: track-1-start / track-2-end; grid-row: time-1400 / time-1530;">
                        <h3 class="session-title">Posters and Demos</h3>
                        <span class="session-time">14:00 - 15:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1530;">15:30</p>

                    <div class="session session-10 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1530 / time-1630;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">15:30 - 16:30</span>
                    </div>

                    <div class="session session-11 track-panel" style="grid-column: track-2-start / track-2-end; grid-row: time-1530 / time-1700;">
                        <h3 class="session-title"><a href="/2021/program/panels/#P2">Panel: Shaping the Future of XR and Arts</a></h3>
                        <span class="session-time">15:30 - 17:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1630;">16:30</p>

                    <div class="session session-12 track-break" style="grid-column: track-1-start / track-1-end; grid-row: time-1630 / time-1700;">
                        <h3 class="session-title">Break</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>

                    <div class="session session-13 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1700 / time-1800;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">17:00 - 18:00</span>
                    </div>

                    <div class="session session-14 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1700 / time-1800;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">17:00 - 18:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>
                    <div class="session session-15 track-event" style="grid-column: track-1-start / track-2-end; grid-row: time-1800 / time-1900;">
                        <h3 class="session-title">Mixer</h3>
                        <span class="session-time">18:00 - 19:00</span>
                    </div>

                </div>

            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible5" class="toggle" type="checkbox" checked> <label for="collapsible5" class="lbl-toggle">Thursday, April 1</label>
        <div class="collapsible-content">
            <div class="content-inner">

                <div class="schedule" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon WEST UTC+1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>

                    <p class="time-slot" style="grid-row: time-0830;">8:30</p>

                    <div class="session session-1 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">8:30 - 9:30</span>
                    </div>

                    <div class="session session-2 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">8:30 - 9:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-0930;">09:30</p>
                    <div class="session session-3 track-event" style="grid-column: track-1-start / track-2-end; grid-row: time-0930 / time-1030;">
                        <h3 class="session-title">BOF/Social</h3>
                        <span class="session-time">9:30 - 10:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1030;">10:30</p>
                    <div class="session session-4 track-orange" style="grid-column: track-1-start / track-2-end; grid-row: time-1030 / time-1200;">
                        <h3 class="session-title">Posters and Demos</h3>
                        <span class="session-time">10:30 - 12:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>

                    <div class="session session-5 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">12:00 - 13:00</span>
                    </div>

                    <div class="session session-5 track-panel" style="grid-column: track-2-start / track-2-end; grid-row: time-1200 / time-1330;">
                        <h3 class="session-title"><a href="/2021/program/panels/#P3">Panel: What makes a virtual human human?</a></h3>
                        <span class="session-time">12:00 - 13:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <div class="session session-7 track-break" style="grid-column: track-1-start / track-1-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Lunch</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>

                    <div class="session session-8 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title">Paper Session</h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>

                    <div class="session session-9 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1500;">
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

                    <div class="session session-2 track-teal" style="grid-column: track-1-start / track-2-end; grid-row: time-1630 / time-1800;">
                        <h3 class="session-title"><a href="#">Closing</a></h3>
                        <span class="session-time">16:30 - 18:00</span>
                    </div>

                </div>

            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible6" class="toggle" type="checkbox" checked> <label for="collapsible6" class="lbl-toggle">Friday, April 2</label>
        <div class="collapsible-content">
            <div class="content-inner">

                <div class="schedule-fri-2" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;">Lisbon WEST UTC+1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;">Track 1</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;">Track 2</span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;">Track 3</span>

                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>
                    <div class="session session-1 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#WEVR">Workshop: Everyday Virtual Reality (WEVR)</a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>
                    <div class="session session-2 track-teal" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1630;">
                        <h3 class="session-title"><a href="#">Tutorial: bmlTUX – a simple toolkit for building experiments in Unity</a></h3>
                        <span class="session-time">14:00 - 16:30</span>
                    </div>
                    <div class="session session-3 track-teal" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1630;">
                        <h3 class="session-title"><a href="#">Tutorial: Emotion in Virtual Reality</a></h3>
                        <span class="session-time">14:00 - 16:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>
                    <div class="session session-4 track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-1600 / time-2100;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#KELVAR">Workshop: K-12+ Embodied Learning through Virtual and Augmented Reality</a></h3>
                        <span class="session-time">16:00 - 21:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>
                    <div class="session session-5 track-teal" style="grid-column: track-1-start / track-1-end; grid-row: time-1700 / time-2000;">
                        <h3 class="session-title"><a href="#">Tutorial: OpenAR: Combining the Virtual and Real?</a></h3>
                        <span class="session-time">17:00 - 20:00</span>
                    </div>
                    <div class="session session-6 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1700 / time-2100;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#Finding-a-way-forward-in-VR-locomotion">Workshop: Finding a way forward in VR locomotion</a></h3>
                        <span class="session-time">17:00 - 21:00</span>
                    </div>
                </div>

            </div>
        </div>
    </div>
</div>




<!--
<div>
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
</div>
    -->



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
