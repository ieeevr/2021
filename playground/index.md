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

        width: 100%;
        margin-left: auto;
        margin-right: auto;
    }

    .styled-table thead tr {
        background-color: #00aeef;
        color: #ffffff;
        text-align: left;
    }

    .styled-table th,
    .styled-table td {
        padding: 12px 15px;
        width: 25%;
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

    < !-- div {
        text-align: justify;
        text-justify: inter-word;
    }

    -->

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

    /* Thumbnails box */
    .box {
        border-radius: 5px;
        padding: 20px;
    }

    .box:nth-child(even) {
        color: red;
    }

    .wrapper {
        display: grid;
        /* border: 1px solid #000; */
        grid-gap: 10px;
        grid-template-columns: repeat(auto-fill, 150px 30%);
    }

    .letter {
        border: solid 1px #656565;
        border-radius: 5px;
        /*font-family: 'Courier New', monospace;*/
        font-family: 'Times New Roman', serif;
    }

</style>


<div style="border: solid 1px #656565; border-radius: 5px;">
    <div style="padding: 30px 30px 30px 30px;">
        <p>
            To our Exhibitor and Sponsors,
        </p>
        <p>
            We’d like to extend our deep gratitude to the exhibitors and sponsors who have partnered with us for the 2021 IEEE VR Conference.
        </p>
        <p>
            The important partnerships, which foster collaboration and sharing trusted research, helps further the educational and global objectives of IEEE VR that our community and the field-at-large depend on.
        </p>
        <p>
            Because of their participation and connection with the IEEE VR community, our conference was able to provide much-needed scholarships to students, offer student mentorship programs, contribute to the expanding access to our conferences, and make computing research and information available to a wider audience, allowing us to share important developments across the globe.
        </p>
        <p>
            We remain dedicated to ensuring that our partnerships deliver rich opportunities for each supporter, including building impactful relationships, strengthening their workforce, and expanding their brand’s reach, all critical objectives for competitive computing technologies.
        </p>
        <p>
            We sincerely appreciate the collaboration and partnerships we’ve achieved and the positive impact that they’ve each made on the community.
            Many thanks,
        </p>
        <p>
            The IEEE VR 2021 Conference Committee
        </p>
    </div>
</div>
