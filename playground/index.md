---
layout: ieeevr-default
title: "Call for Exhibitors and Sponsors"
---

<style>
    <style>* {
        box-sizing: border-box;
    }

    .exhibitors-center {
        margin: auto;
        width: 90%;
    }

    .exhibitors-row {
        display: flex;
        background-color: #00aeef;
        border-radius: 10px;
        padding: 10px;
    }

    .exhibitors-column {
        flex: 50%;
        padding: 20px;
        position: relative;
    }

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
        padding: 0.1rem;
        color: #00aeef;
        background: #ffffff;
        cursor: pointer;
        border-radius: 7px;
        transition: all 0.25s ease-out;
    }

    .lbl-toggle:hover {
        /*color: #FFF;*/
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

    /* THUMBNAILS*/
    .list {
        max-width: 1400px;
        margin: 20px auto;
    }

    .img-list a {
        text-decoration: none;
    }

    .li-sub p {
        margin: 0;
    }

    .list li {
        border-bottom: 1px solid #ccc;
        display: table;
        border-collapse: collapse;
        width: 100%;
    }

    .inner {
        display: table-row;
        overflow: hidden;
    }

    .li-img {
        display: table-cell;
        vertical-align: middle;
        width: 25%;
        padding-right: 1em;
    }

    .li-img img {
        display: block;
        width: 100%;
        height: auto;

    }

    .li-text {
        display: table-cell;
        vertical-align: middle;
        width: 75%;
    }

    .li-head {
        margin: 10px 0 0 0;
    }

    .li-sub {
        margin: 0;
    }

    @media all and (min-width: 45em) {
        .list li {
            float: left;
            width: 50%;
        }
    }

    @media all and (min-width: 75em) {
        .list li {
            width: 33.33333%;
        }
    }

    /* for flexbox */
    @supports(display: flex) {
        .list {
            display: flex;
            flex-wrap: wrap;
        }

        .li-img,
        .li-text,
        .list li {
            display: block;
            float: none;
        }

        .li-img {
            align-self: center;
            /* to match the middle alignment of the original */
        }

        .inner {
            display: flex;
        }
    }

    /* for grid */
    @supports(display: grid) {
        .list {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(400px, 1fr));
        }

        .list li {
            width: auto;
            /* this overrides the media queries */
        }
    }

    /* video container */
    .video-container {
        overflow: hidden;
        position: relative;
        width: 100%;
    }

    .video-container::after {
        padding-top: 56.25%;
        /* 75% if 4:3*/
        display: block;
        content: '';
    }

    .video-container iframe {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
    }

</style>

<div>
    <h1>Exhibitors and Sponsors</h1>


    <div class="notice--info">
        <p><strong>
                Please click <a href="/2021/contribute/exhibitors/">HERE</a> for more exhibit and sponsor information.
            </strong>
        </p>
    </div>

    <table class="styled-table" style="font-size: 0.8em;">
        <tr>
            <th>Dedicated exhibit hours </th>
            <th>(Lisbon WEST UTC+1)</th>
        </tr>
        <tr>
            <td>Monday, March 29</td>
            <td><a href="/2021/program/overview/#EX1">16:00 - 17:30</a></td>
        </tr>
        <tr>
            <td>Tuesday, March 30</td>
            <td><a href="/2021/program/overview/#EX2">10:30 - 12:30</a><br /><a href="/2021/program/overview/#EX3">17:00 - 18:30</a></td>
        </tr>
        <tr>
            <td>Wednesday, March 31</td>
            <td><a href="/2021/program/overview/#EX4">10:30 - 11:30</a><br /><a href="/2021/program/overview/#EX5">15:00 - 16:00</a></td>
        </tr>
        <tr>
            <td>Thursday, April 1</td>
            <td><a href="/2021/program/overview/#EX6">11:30 - 13:00</a><br /><a href="/2021/program/overview/#EX7">17:30 - 18:30</a></td>
        </tr>

        <tr>
            <th>Welcome Reception</th>
            <th>(Lisbon WEST UTC+1)</th>
        </tr>
        <tr>
            <td>Monday, March 29</td>
            <td><a href="/2021/program/overview/#EXW">18:00 - 19:30</a></td>
        </tr>

    </table>
</div>

<div>

    <h2>
        <a href="https://www.virbela.com/" target="_blank">
            <img style="width: 20%;" src="/2021/assets/images/sponsors/Virbela-logo.png" alt="Virbela Logo">
        </a>
    </h2>
    <div class="video-container">
        <iframe src="https://www.youtube.com/embed/TuOBgzJeQj0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

</div>

<div>
    <h2>Literature Distribution</h2>
    <p>Please click on the companies below to access more content from this year's exhibitors.</p>



    <ul class="list img-list">

        <li>
            <a href="#" class="inner">
                <div class="li-img">
                    <img src="/2021/assets/exhibitors/Appen-Augmented-and-Virtual-Reality-One%20Pager.png" />
                </div>
                <div class="li-text">
                    <h3 class="li-head">Appen</h3>
                    <div class="li-sub">
                        <a href="/2021/assets/exhibitors/Appen-Augmented-and-Virtual-Reality-One%20Pager.pdf" target="_blank">
                            <p>Augmented and Virtual Reality</p>
                        </a>
                    </div>
                </div>
            </a>
        </li>
        <li>
            <a href="#" class="inner">
                <div class="li-img">
                    <img src="/2021/assets/exhibitors/HITLabNZ_Brochure.png" />
                </div>
                <div class="li-text">
                    <h3 class="li-head">HIT Lab NZ</h3>
                    <div class="li-sub">
                        <a href="/2021/assets/exhibitors/HITLabNZ_Brochure.pdf" target="_blank">
                            <p>Human Interface Technology<br />We put people before technology</p>
                        </a>
                    </div>
                </div>
            </a>
        </li>
        <li>
            <a href="#" class="inner">
                <div class="li-img">
                    <img src="/2021/assets/exhibitors/IEEE_VR_2021-Microsoft.png" />
                </div>
                <div class="li-text">
                    <h3 class="li-head">Microsoft</h3>
                    <div class="li-sub">
                        <a href="/2021/assets/exhibitors/IEEE_VR_2021-Microsoft.pdf" target="_blank">
                            <p>Microsoft Mixed Reality</p>
                        </a>
                    </div>
                </div>
            </a>
        </li>
        <li>
            <a href="#" class="inner">
                <div class="li-img">
                    <img src="/2021/assets/exhibitors/Qualcomm-Virtual-Recruiting-Guide.png" />
                </div>
                <div class="li-text">
                    <h3 class="li-head">Qualcomm</h3>
                    <div class="li-sub">
                        <a href="/2021/assets/exhibitors/Qualcomm-Virtual-Recruiting-Guide.pdf" target="_blank">
                            <p>Virtual Recruiting Guide</p>
                        </a>
                    </div>
                </div>
            </a>
        </li>
    </ul>



</div>




    <ul class="list img-list">
        <li>
            <a href="#" class="inner">
                <div class="li-img">
                    <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/12005/balloon-sq1.jpg" alt="Hot air balloons" />
                </div>
                <div class="li-text">
                    <h3 class="li-head">Title of Content</h3>
                    <div class="li-sub">
                        <p>Summary of content.</p>
                    </div>
                </div>
            </a>
        </li>
        <li>
            <a href="#" class="inner">
                <div class="li-img">
                    <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/12005/balloon-sq2.jpg" alt="Hot air balloons" />
                </div>
                <div class="li-text">
                    <h3 class="li-head">Title of Content</h3>
                    <div class="li-sub">
                        <p>Summary of content.</p>
                    </div>
                </div>
            </a>
        </li>
        <li>
            <a href="#" class="inner">
                <div class="li-img">
                    <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/12005/balloon-sq3.jpg" alt="Hot air balloons" />
                </div>
                <div class="li-text">
                    <h3 class="li-head">Title of Content</h3>
                    <div class="li-sub">
                        <p>Summary of content.</p>
                        <p>Sometimes we get more content than we expected.</p>
                        <p>The design should cope with this!</p>
                    </div>
                </div>
            </a>
        </li>
        <li>
            <a href="#" class="inner">
                <div class="li-img">
                    <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/12005/balloon-sq13.jpg" alt="Hot air balloons" />
                </div>
                <div class="li-text">
                    <h3 class="li-head">Title of Content</h3>
                    <div class="li-sub">
                        <p>Summary of content.</p>
                    </div>
                </div>
            </a>
        </li>
    </ul>
