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
        width: 30%;
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
        width: 70%;
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

</style>

<h2>Literature Distribution</h2>
<p>Please click on the companies below to access more content from this year's exhibitors.</p>


<div class="wrap-collabsible"> <input id="collapsible1" class="toggle" type="checkbox" checked> <label for="collapsible1" class="lbl-toggle">Appen</label>
    <div class="collapsible-content">
        <div class="content-inner">


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
        </div>
    </div>
</div>
<div class="wrap-collabsible"> <input id="collapsible1" class="toggle" type="checkbox" checked> <label for="collapsible2" class="lbl-toggle">HIT Lab NZ</label>
    <div class="collapsible-content">
        <div class="content-inner">


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
        </div>
    </div>
</div>
<div class="wrap-collabsible"> <input id="collapsible1" class="toggle" type="checkbox" checked> <label for="collapsible3" class="lbl-toggle">Microsoft</label>
    <div class="collapsible-content">
        <div class="content-inner">


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
        </div>
    </div>
</div>
<div class="wrap-collabsible"> <input id="collapsible1" class="toggle" type="checkbox" checked> <label for="collapsible3" class="lbl-toggle">Qualcomm</label>
    <div class="collapsible-content">
        <div class="content-inner">


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
        </div>
    </div>
</div>

