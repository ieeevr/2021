---
layout: ieeevr-default
title: "VGTC Award Winners"
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
        width: 50%;
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

    .styled-table2 {
        border-collapse: collapse;
        margin: 25px 0;
        font-size: 0.8em;
        font-family: sans-serif;
        /*min-width: 400px;*/
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
        display: table;
        width: 50%;
        margin-left: auto;
        margin-right: auto;


    }

    .styled-table2 thead tr {
        background-color: #00aeef;
        color: #ffffff;
        text-align: left;
    }

    .styled-table2 th,
    .styled-table2 td {
        padding: 12px 15px;
        width: 50%;
    }

    .styled-table2 tbody tr {
        border-bottom: 1px solid #dddddd;
    }

    .styled-table2 tbody tr:nth-of-type(even) {
        background-color: #f3f3f3;
    }

    .styled-table2 tbody tr:last-of-type {
        border-bottom: 2px solid #00aeef;
    }

    .styled-table2 tbody tr.active-row {
        font-weight: bold;
        color: #00aeef;
    }

    img {
        display: block;
        margin-left: auto;
        margin-right: auto;
    }

    /*
    div {
        text-align: justify;
        text-justify: inter-word;
    }
    */

</style>


<h1>VGTC Awards</h1>

<p>The IEEE VGTC Virtual and Augmented Reality Technical Awards program recognizes individuals who have made a significant contribution to the community through their research. </p>


<div>
<!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'O2' %}
    {% if event.location %}
    <div class="notice--info">
        <strong style="padding-bottom: 5px;">Take me to the event:</strong>
        <p>
            <strong style="color: black;">Virbela Location:</strong> {{ event.location }} (<a href="/2021/attend/virbela-instructions/#map">MAP</a>)

            {% if event.stream-url %}
            <br />
            {% if event.aindanaoaconteceu %}
            <strong style="color: black;">Watch video stream live:</strong> <a href="{{ event.stream-url }}" target="_blank">HERE</a>
            {% else %}
            <strong style="color: black;">Watch the recorded video stream:</strong> <a href="{{ event.stream-url }}" target="_blank">HERE</a>
            {% endif %}
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
</div>


<div>

    <center>
        <h2>The 2021 VGTC Virtual Reality Career Award</h2>
    </center>
    <center><strong>Mary Whitton</strong></center>
    <br />

    <img src="/2021/assets/images/Images_VGTC_Awards/image1.png" alt="Mary Whitton">

    <br />


    <p>The 2021 IEEE VGTC Virtual Reality Career Award goes to Mary C. Whitton in recognition of her lifetime contributions to the technologies, techniques, and theory that enable virtual and mixed reality systems and applications to better achieve their intended goals. Throughout her career, she has applied the technical rigors of engineering and psychological measurement to evaluating and improving the user experience in VR and MR. As an entrepreneur, Whitton designed innovative hardware components for interactive 3D graphics and focused on the user benefits of her companies’ pioneering technologies. As co-lead, with Fred Brooks, of the Effective Virtual Environments (EVE) research team at UNC-Chapel Hill, she and her students applied knowledge of hardware, human perception, and user evaluation to improving virtual and mixed reality experiences. The EVE group launched the research areas of Redirected Walking and Passive Haptics and was a pioneer in the use of physiological measures to evaluate stress-inducing virtual environments.</p>

    <p><strong>Bio</strong></p>

    <p>
        Mary C. Whitton is a research professor (retired) of computer science at the University of North Carolina at Chapel Hill. She has worked in the areas of interactive 3D computer graphics and virtual and mixed reality since 1976. It was then that she left public school teaching to study computer graphics at North Carolina State University where she joined Prof. John Staudhammer’s pioneering graphics research group. Having earned M.S. degrees in Guidance and Personnel Services (Counseling) (1974) and in Electrical and Computer Engineering (1984) from NCSU, Whitton’s lifetime work is deeply grounded in both graphics systems technology and the human-centered discipline of psychological measurement.
    </p>
    <p>
        Interrupting her formal education, Professor Whitton, with her husband Nick England, co-founded Ikonas Graphics Systems (1978) and Trancept Systems (1986). Both companies designed and sold highend, user-programmable graphics hardware and libraries for graphics, image processing, volume rendering, and visualization. The companies’ products were widely adopted in academic and industrial research laboratories for applications including seismic exploration, 3D medical imaging, intelligence analysis, computer animation, and scientific modeling and simulation. The Ikonas RDS-3000 is the ancestor of today’s programmable graphics processing units, even though it was about the size of a dorm refrigerator. As Ikonas’ primary contact with customers from many disciplines, Whitton developed a keen sense of the user’s perspective.
    </p>
    <p>
        After joining UNC-Chapel Hill in 1994, Whitton co-led the Effective Virtual Environments (EVE) research group that developed and evaluated technologies to make virtual environment systems more effective for applications such as simulation, training, and rehabilitation. The fundamental questions that drove EVE research (1996–2016) were: What are the characteristics of hardware, software, and applications that make virtual environments successful; what techniques can researchers invent or improve, and then use, to make VEs more successful; and how should developers measure “success”? These questions led to groundbreaking work in redirected walking and passive haptics, and studies to understand the extent to which VR systems and interface techniques could fool the visual and tactile senses.
    </p>
    <p>

        Whitton collaborated with UNC colleagues, frequently Henry Fuchs, on multiple augmented and mixed reality projects. In the early 2000s, Whitton led a multi-disciplinary team that designed and evaluated the distributed Nanomanipulator system, a distributed collaboration system for multi-modal, mixed-reality scientific data exploration.
        Throughout her decades of pioneering work, Professor Whitton has mentored generations of students at UNC-Chapel Hill and from other university research groups with whom she collaborated.</p>
    <p>

        Building on student work that proposed the construct of <i>coherence</i> as an objective measure for VR’s Plausibility Illusion, Whitton’s most recent collaborative work reexamines and proposes revisions to Milgram and Kishino’s 1994 reality-virtuality continuum and taxonomic framework for VR and MR.</p>
    <p>

        Professor Whitton was President of the ACM SIGGRAPH organization from 1993 to 1995, and the recipient of the 2013 SIGGRAPH Outstanding Service Award. She is a Life Senior Member of IEEE and currently serves on the Steering Committee for the IEEE Virtual Reality Conference. In her retirement, she enjoys spending time with ACM committees working on preserving computer graphics history.
    </p>

    <strong>Award Information</strong><br />

    <p>The IEEE VGTC Virtual Reality Career Award was established in 2005. It is given every year to an individual to honor that person’s lifetime contributions to virtual & augmented reality. Nominations for the Virtual Reality Career Award can be submitted to the awards current chair, Henry Fuchs, at vgtc-vr-awards[at]vgtc.org.</p>

</div>

<div>

    <center>
        <h2>The 2021 VGTC Virtual Reality Technical Achievement Award</h2>
    </center>
    <center><strong>David P. Luebke</strong></center>
    <br />
    <img src="/2021/assets/images/Images_VGTC_Awards/image2.png" alt="David P. Luebke" width="50%">

    <br />

    <!-- <center><big><strong>{{ keynote.title }}</strong></big></center> -->
    <!-- <center><small>{{ keynote.day }} - {{ keynote.start }}, {{ keynote.timezone }}</small></center> -->


    <p>
        The 2021 IEEE VGTC Virtual Reality Technical Achievement Award goes to David Luebke of NVIDIA, in recognition of his research and leadership at the intersection of rendering algorithms, display technology, and human perception. With an interdisciplinary orientation, Dr. Luebke and his team have advanced the state of virtual reality across topics as diverse as real-time rendering, low-latency display, foveated resolution, redirected walking, haptics, and focus-supporting displays.

    </p>

    <p>
        <strong>Bio</strong>
    </p>
    <p>

        David Luebke has been researching and leading research teams on topics relevant to Virtual Reality since his first published paper in 1995. Originally a chemist by training, he was inspired by the concept of VR to switch fields and pursue graduate work in computer graphics at the University of North Carolina. Finding that graphics horsepower was the primary technical factor limiting VR performance, Luebke focused his early research on algorithms for accelerating real-time rendering. At the University of Virginia, Luebke continued his real-time rendering research, putting it into VR practice with UNC colleagues in the large-scale 2003 museum exhibit “Virtual Monticello”. During this time, Luebke also became interested in general-purpose GPU computing and in guiding rendering with human visual perception, beginning with a foveated rendering system published in 2001. Arriving at NVIDIA in 2006, Luebke unified these interests in helping to establish GPU ray tracing research and products, and also began work on what he perceived as the new bottleneck of VR systems: display technology. Starting with a seminal 2013 paper on near-eye light field displays, Luebke has focused on the co-design of optics, display electronics, and rendering algorithms that match the constraints and opportunities of human vision. Most recently, Luebke’s team has also focused on using generative deep neural networks for photorealistic human avatars.
    </p>
    <p>

        David Luebke is the vice president of graphics research at NVIDIA, where he was a founding member of NVIDIA Research in 2006. He earned a B.A. <i>magna cum laude</i> in Chemistry from Colorado College in 1993, and an M.S. in 1997 and Ph.D. in 1998 under the supervision of Frederick P. Brooks, Jr. from the University of North Carolina at Chapel Hill. He joined the faculty of the Department of Computer Science at the University of Virginia that same year, where he received a National Science Foundation CAREER Award and the parallel Department of Energy Early Career Principal Investigator award, as well as multiple awards and fellowships for undergraduate teaching. After eight years Luebke left Virginia to join NVIDIA as a founding member of NVIDIA Research, where he now leads a longterm research group spanning all aspects of computer graphics.
    </p>
    <p>

        Together with his colleagues, Luebke has co-authored a book on mesh simplification techniques, a SIGGRAPH Electronic Theater piece on realistic human skin rendering, a major New Orleans Museum of Art exhibit (visited by over 110,000 people) on Thomas Jefferson’s Monticello, several SIGGRAPH Emerging Technologies exhibits on display technology for virtual and augmented reality, and approximately two hundred papers, articles, chapters, and patents. He was instrumental in the development of NVIDIA GPU ray tracing technology, embodied in the 2009 release of the NVIDIA OptiX software platform and the 2018 release of the NVIDIA RTX hardware platform, showcased in NVIDIA’s 20X0 “Turing” GPUs. Luebke is a Fellow of the IEEE. His other honors include the NVIDIA Distinguished Inventor award, the aforementioned NSF CAREER and DOE ECPI awards, and the ACM Symposium on Interactive 3D Graphics “Test of Time Award” for that first 1995 paper motivated by efficient rendering for VR architectural walkthroughs.

    </p>

    <p>
        <strong>Award Information</strong><br />
        The IEEE VGTC Virtual Reality Technical Achievement Award was established in 2005. It is given every year to recognize an individual for a seminal technical achievement in virtual and augmented reality. VGTC members may nominate individuals for the Virtual Reality Technical Achievement Award by contacting the awards chair, Henry Fuchs, at vgtc-vr-awards[at]vgtc.org

    </p>

</div>

<hr>
