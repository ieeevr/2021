---
layout: ieeevr-default
title: "Workshop Papers"
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
    <h1 id="call-for-workshop-papers"> Workshops </h1>
    <p>
        The following 14 workshops will be held at IEEE Virtual Reality 2021. The workshops will be held on March 27-28 and April 2-3, 2021
    </p>
    
    <table class="styled-table">

        <tr>
            <th>Workshops</th>
        </tr>
        {% for workshop in site.data.workshops %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ workshop.id }}">{{ workshop.title }}</a></td>
        </tr>
        {% endfor %}
    </table>

    <h2 id="TrainingXR"> 2nd Annual Workshop on 3D Content Creation for Simulated Training in eXtended Reality (TrainingXR) </h2>
    
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'TrainingXR-1' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/trainingxrieeevr2021" target="_blank"> https://sites.google.com/view/trainingxrieeevr2021 </a>
    </p>
    <ul>
        <li> Submission deadline 25/01/2021 </li>
        <li> Notification 31/01/2021 </li>
        <li> Camera-ready submission 12/02/2021 </li>
    </ul>
    <p>
        This workshop discusses and articulates research visions on using the latest extended reality (VR/AR/MR) technologies for education and training purposes, and on creating immersive 3D virtual content for delivering effective and personalized training experiences. This workshop will gather researchers and practitioners in a variety of computer disciplines related to XR training and content creation. This workshop will accept research papers on these topics. We will also invite renowned speakers from the research community and the industry to give talks related to XR-based training to inspire the field to further explore this promising direction.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Lap-Fai (Craig) Yu
    </p>

    <h2 id="SeatedVR"> Seated Virtual Reality & Embodiment (SeatedVR) </h2>
    
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'SeatedVR' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/seated-vr/home" target="_blank">https://sites.google.com/view/seated-vr/home</a>
    </p>
    <ul>
        <li> Submission deadline <del>20/01/2021</del> 24/01/2021 </li>
        <li> Notification 31/01/2021 </li>
        <li> Rebuttal (short papers) 05/02/2021 </li>
        <li> Final notification (short papers) 08/02/2021 </li>
        <li> Camera-ready submission 10/02/2021 </li>
    </ul>
    <p>
        In this highly interactive workshop we want to discuss topics in the scenario of seated virtual reality, with this year’s edition having a special focus on embodiment. This means next to comfort, postural conflicts & transitions, we also want to investigate the special role of embodied interaction when the user is potentially less engaged: sitting on her/his couch, sofa or office chair, a situation that might have even more often occurred in these times of the pandemic. As last year, we want only a small part of the workshop to be covered by lightning talks to have time for an interactive discussion session.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Daniel Zielasko
    </p>

    <h2 id="SIVE"> Sonic Interactions in Virtual Environments (SIVE) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'SIVE' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sive.create.aau.dk/" target="_blank">https://sive.create.aau.dk/</a>
    </p>
    <ul>
        <li> Abstract submission 15/01/2021 </li>
        <li> paper submission deadline 20/01/2021 </li>
        <li> Notification 31/01/2021 </li>
        <li> Camera-ready submission 12/02/2021 </li>
    </ul>
    <p>
        The main goal of this workshop is to increase among the virtual reality community the awareness of the importance of sonic elements when designing virtual/augmented/mixed reality environments (XR hereafter). We will also discuss how research in other related fields such as film sound theory, product sound design, sound and music computing, game sound design and computer music can inform designers of XR environments. Moreover, the workshop will feature state of the art research on the field of sound for XR environments.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Stefania Serafin
    </p>

    <h2 id="VHCIE2021"> 6th Workshop on Virtual Humans and Crowds for Immersive Environments (VHCIE 2021) </h2>
    
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'VHCIE2021' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="http://files.inria.fr/vhcie/" target="_blank">http://files.inria.fr/vhcie/</a>
    </p>
    <ul>
        <li> Submission deadline 17/01/2021 </li>
        <li> Notification 31/01/2021 </li>
        <li> Camera-ready submission 12/02/2021 </li>
    </ul>
    <p>
        VHCIE (Virtual Humans and Crowds in Immersive Environments) is a half-day workshop associated with the IEEE VR CONFERENCE that aims at presenting state of the art character and crowd animation techniques for interactive characters, examples of new research opportunities by the availability of populating virtual environments, new research on avatars as well as discussing technological requirements for future applications.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Anne-Hélène Olivier
    </p>

    <h2 id="WISP"> Workshop on Immersive Sickness Prevention (WISP) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'WISP' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/umn.edu/wisp" target="_blank">https://sites.google.com/umn.edu/wisp</a>
    </p>
    <ul>
        <li> Submission deadline 31/01/2021 </li>
        <li> Notification 07/02/2021 </li>
        <li> Camera-ready submission 12/02/2021 </li>
    </ul>
    <p>
        The Workshop on Immersive Sickness Prevention is intended to foster discussion between researchers, developers, and practitioners interested in addressing cybersickness, one of the most significant usability issues in the virtual reality field. Although immersive technologies have been advancing rapidly, their rate of public adoption has been slowed by the fact that many users experience physical discomfort during or after the use of VR devices, with symptomatic characteristics similar to motion sickness. Furthermore, studies have consistently shown that motion sickness disproportionately affects women, and concerns have been raised about the existence of inequitable barriers for engaging with immersive media. The workshop program will include primary research papers that report study results, novel interaction techniques, or technological interventions aimed towards understanding and mitigating cybersickness, as well as position papers describing early-stage concepts, preliminary results, or case studies from industry.
    </p>
    <p>
        <strong style="color:black;">Principal Organizers:</strong> Evan Suma Rosenberg and Victoria Interrante
    </p>

    <h2 id="NIDIT"> Novel Input Devices and Interaction Techniques – NIDIT </h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'NIDIT' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/nidit" target="_blank">https://sites.google.com/view/nidit</a>
    </p>
    <ul>
        <li> Submission deadline 22/01/2021 </li>
        <li> Notification 31/01/2021 </li>
        <li> Camera-ready submission 12/02/2021 </li>
    </ul>
    <p>
        Virtual reality has finally become a mainstream technology. Recent advances in commercial VR hardware have led to high-resolution, ergonomic, – and critically – low cost head-mounted displays. Advances in commercial input devices and interaction techniques have arguably not kept pace with advances in displays. For instance, most HMDs include a tracked input device: “wands” that are not dissimilar to the earliest examples of 3D controllers used in the VR systems of the 1980s. Interaction in commercial VR systems has similarly lagged; despite many advances in 3D interaction in the past three decades of VR research, interaction in commercial systems largely relies on classical techniques like the virtual hand, or ray-casting. This half-day workshop will bring together researchers and industry practitioners to discuss and experience the future of input devices for VR, AR, and 3D User Interfaces, and help chart a course for the future of 3D interaction techniques.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Robert J. Teather
    </p>

    <h2 id="WEVR"> WEVR: 7th Annual Workshop on Everyday Virtual Reality </h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'WEVR' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://wevr.adalsimeone.me/" target="_blank">https://wevr.adalsimeone.me/</a>
    </p>
    <ul>
        <li> Abstract submission 15/01/2021 </li>
        <li> Paper submission deadline 24/01/2021 </li>
        <li> Notification 31/01/2021 </li>
        <li> Camera-ready submission 12/02/2021 </li>
    </ul>
    <p>
        The WEVR workshop will cover “Everyday” Virtual, Augmented and Mixed Reality research themes in all contexts and scenarios beyond research laboratories and specialist environments. This half-day workshop will bring together researchers and industry practitioners to explore new challenges and define a new research agenda.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Adalberto L. Simeone
    </p>

    <h2 id="KELVAR"> KELVAR: 6th Annual Workshop on K-12+ Embodied Learning through Virtual and Augmented Reality </h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'KELVAR' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/site/vrkelvar/" target="_blank">https://sites.google.com/site/vrkelvar/</a>
    </p>
    <ul>
        <li> Abstract submission 14/01/2021 </li>
        <li> Paper submission deadline 22/01/202 </li>
        <li> Notification 31/01/2021 </li>
        <li> Camera-ready submission 12/02/2021 </li>
    </ul>
    <p>
        K-12+ (K-12 and higher ed) education is currently undergoing a technological revolution creating opportunities for Virtual-, Augmented-, and Mixed-Reality based learning (hereafter referred to as XR [extended reality] technologies. Technology integration will continue to increase as mobile devices penetrate all socioeconomic strata, and as XR technologies become affordable to schools, vocational education providers, universities, and informal educational settings. These technologies have the potential to facilitate effective learning by: developing the ability to engage students of all ages with interactive 3D simulations of real-life and artificial phenomena; presenting information that is spatially – and temporally – integrated with real objects; leveraging whole-body motions to depict and reinforce learning content. However, there are many questions about the integration of such experiences into the classroom, such as: What curriculum topics might be addressed through XR technologies?; What socio-cultural, psychological and physiological mechanisms underlie embodied cognition?; How can we design experiences that are appropriate for the different stages of human development?; How will pedagogical approaches be influenced by such technologies? In this workshop we aim to bring together educators, developers and researchers who are interested in creating and deploying XR technologies for the educational contexts of the future. The workshop will enable participants to discuss and engage with different approaches for designing and integrating XR technologies with a specific focus on the challenges and potential for embodied learning in the classroom for K-12, vocational and higher education.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Steven Cutchin
    </p>

    <h2 id="EXR"> Ethics in XR (EXR)</h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'EXR' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/ethicsinxr/home" target="_blank">https://sites.google.com/view/ethicsinxr/home</a>
    </p>
    <ul>
        <li> Submission deadline <del>25/01/2021</del> 05/02/2021 </li>
        <li> Notification <del>30/01/2021</del>  08/02/2021 </li>
        <li> Camera-ready submission 12/02/2021 </li>
    </ul>
    <p>
        There is an increase in and diversification of XR content with various degrees of interaction, from computer-generated VR to cinematic VR, ranging from games and short films, to serious games and social VR platforms. In the past few years, XR consumption has also diversified with the occurrence of platforms that range from mobile VR to high-end headsets. VR has been consumed more ubiquitously than ever, outside of controlled environments such as research labs and in public places like VR arcades, escape rooms, pubs, film and art festivals. As more and more users come into contact with XR - and given the solid body of research on the effects and role of realism, self representation through avatars, immersion and presence on VR users’ experience - we recognise that there is a need to address potential ethical aspects related to the production and consumption of XR and to discuss the challenges and opportunities that come with the increased popularity of the medium. The Ethics in XR Workshop focuses on addressing various ethical aspects related to the production and consumption of VR, MR, AR and immersive 360-degree content.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Ana-Despina Tudor
    </p>

    <h2 id="DISCE"> Distributed Interactive Systems for Collaborative Experiences (DISCE) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'DISCE' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/disce/home" target="_blank">https://sites.google.com/view/disce/home</a>
    </p>
    <ul>
        <li> Submission deadline 18/01/2021 </li>
        <li> Notification 31/01/2021 </li>
        <li> Camera-ready submission 12/02/2021 </li>
    </ul>
    <p>
        Imagine a world where many people in numerous locations collectively solve complex problems using augmented/virtual reality head-mounted displays. We have seen this type of automation in some industrial research and in a few commercially available applications (e.g., HoloLens Microsoft Dynamics 365). However, some AR/VR applications are network and compute intensive, often exceeding the acceptable latency for interactive systems (app dependent). Since the speed of light limits network communication, merely creating faster networks with more bandwidth will not solve this problem. Instead, we need to find new solutions to improve collaborative systems when using AR/VR, especially when the systems are interactive.This workshop will bring together researchers and industry practitioners to discuss and experience the future of three-dimensional distributed collaborative interactive systems and their challenges.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Francisco R. Ortega
    </p>

    <!--
    <h2 id="Combining-the-Virtual-and-the-Real"> Combining the Virtual and the Real in a World that Works for Everyone </h2>
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://openarcloud/IEEE2021" target="_blank">https://openarcloud/IEEE2021</a>
    </p>
    <ul>
        <li> Call for Participation opens 15/02/2021 </li>
        <li> Submission deadline 22/03/2021 </li>
        <li> Notification rolling acceptance </li>
    </ul>
    <p>
        Open AR Cloud's mission is to drive the development of open and interoperable spatial computing technology, data and standards to connect the physical and digital worlds for the benefit of all. It is essential that the Open Spatial Computing Platform (OSCP) is designed for all of humanity in all its diversity and does not become a walled garden controlled by one or a few large corporations. Many of the world’s largest companies are currently investing heavily in this type of technology, but they might not be the best custodians of important things like the rights to privacy and freedom of individuals. Designing and building a reference implementation of the OSCP would be ambitious for any organization. We fully realize we must extend our team, scale up our operation and raise funding to be able to achieve the “Minimal Viable Platform” we have outlined at https://www.openarcloud.org/oscp. We are excited about the people and partners already part of this journey, but we need more hands on deck and more rocket fuel to power this mission! This is where you or your organization enters the stage. This series of presentations, immersive QandA sessions, and live hands-on workshops with our most seasoned developers will give you what you need to make a contribution to this impending technical revolution. Even if you don’t code, join us to learn about opportunities to become a part of the Open Ar Coud’s solution. Don’t let this chance to do something exciting, meaningful and important pass you by!
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Suzan Oslin
    </p>
    -->

    <h2 id="Finding-a-way-forward-in-VR-locomotion"> Finding a way forward in VR locomotion </h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'Finding-a-way-forward-in-VR-locomotion' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://locomotionvault.github.io/workshopieeevr.html" target="_blank">https://locomotionvault.github.io/workshopieeevr.html</a>
    </p>
    <ul>
        <li> Submission deadline 29/01/2021 </li>
        <li> Notification 31/01/2021 </li>
        <li> Camera-ready submission 10/02/2021 </li>
    </ul>
    <p>
        In the last decade, numerous Virtual Reality (VR) locomotion techniques (LTs) have been invented, reinvented, combined and modified. Each of the LTs has a unique mix of idiosyncratic characteristics. Newly proposed LTs are usually compared to one or a few other LTs to find their advantages and disadvantages. Researchers have proposed several taxonomies and criteria for describing and evaluating LTs (e.g. in terms of the hardware employed, their granularity, accessibility, etc.). Yet, no agreement exists on which evaluation criteria or taxonomies are the most important when selecting an LT or designing a new one. Our goal is to unify research in the field by creating shared communitysourced evaluation criteria and datasets for locomotion in VR. To this end, we have created LocomotionVault (https://locomotionvault.github.io/. ), an interactive visual database of more than one hundred VR LTs from academia and industry. Each LT is described according to numerous attributes that we collated from existing VR taxonomies which give a similarity score between techniques. In this workshop, we aim to bring VR locomotion researchers together to discuss existing taxonomies and evaluation criteria for VR LTs, challenges in design and evaluation of LTs in such a rapidly-growing space, and potential community-driven tools and initiatives that can move the field forward. We aim to tackle these important topics with talks of the accepted abstracts followed by lively discussions with the attendees.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Mar Gonzalez-Franco
    </p>

    <h2 id="PrXR"> PrXR: Towards a roadmap for privacy and security research for mixed reality applications </h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'PrXR' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://jainlab.cise.ufl.edu/PrXR_2021.html" target="_blank">https://jainlab.cise.ufl.edu/PrXR_2021.html</a>
    </p>
    <ul>
        <li> Submission deadline 24/01/2021 </li>
        <li> Notification 29/01/2021 </li>
        <li> Camera-ready submission 12/02/2021 </li>
    </ul>
    <p>
        This workshop brings together researchers and practitioners in the mixed reality and privacy and security communities to brainstorm threats, threat vectors and consequent opportunities for privacy and security research in the VR/AR/MR community. We will invite speakers from both communities to seed the discussion with their perspectives. The goal of this workshop will be to create a research vision to inspire the community and to catalyze the exploration of a new scientific frontier.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Eakta Jain
    </p>

    <h2 id="ANIVAE"> Animation in Virtual and Augmented Environments - ANIVAE </h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
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
            {% if event.discordurl %}
            <br />
            <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
            {% endif %}
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}
    <!-- TAKE ME TO THE EVENT END-->
    
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://anivae.fhstp.ac.at/" target="_blank">https://anivae.fhstp.ac.at/</a>
    </p>
    <ul>
        <li> Submission deadline 10/01/2021 </li>
        <li> Notification 31/01/2021 </li>
        <li> Camera-ready submission 07/02/2021 </li>
    </ul>
    <p>
        Connecting specialists from various digital humanities research areas (such as animation, games and media studies), with experts from both vision-oriented computer science areas (such as computer graphics or information visualization), and experts from technically-oriented computer science areas (such as data integration, internet-of-things or smart automation), the ANIVAE workshop aims to create an open and exciting environment. By encouraging synergies of interdisciplinary approaches, the workshop maps animation within the AVR context from different angles and creates new knowledge in this research field. ANIVAE wants to account the state-of-the-art research in digital humanities with (software) design and visualization for AVR systems, to shape a common understanding, to compare systems and approaches and derive common paradigms, to develop useful and necessary methods and techniques, and to foster new ideas.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Thomas Moser
    </p>

</div>
