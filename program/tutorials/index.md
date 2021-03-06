---
layout: ieeevr-default
title: "Tutorials"
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
    <table class="styled-table">

        <tr>
            <th>Tutorials</th>
        </tr>
        {% for tutorial in site.data.tutorials %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ tutorial.id }}">{{ tutorial.title }}</a></td>
        </tr>
        {% endfor %}
    </table>
</div>

<div>
    {% for tutorial in site.data.tutorials %}
    {% if tutorial.id == 'T1' %}
    <h2 id="{{ tutorial.id }}">{{ tutorial.title}}</h2>

    <p>
        <strong>Organizers</strong>
    </p>
    <p>
        Evan Suma Rosenberg, University of Minnesota, suma[at]umn.edu<br />
        Blair MacIntyre, Georgia Institute of Technology, blair[at]cc.gatech.edu<br />
    </p>
    <p>
    <strong style="font-size: 0.8em;color: black"> {{ tutorial.schedule1 }}, {{ tutorial.timezone1 }}</strong>
    </p>
    <p>
        This tutorial will teach attendees how to develop web-based virtual reality (VR) experiences and design instructional content for teaching 3D user interface (3DUI) concepts in a remote learning modality. The tutorial content is based upon the instructors' experiences teaching Virtual Reality and 3D User Interfaces at the University of Minnesota and at Georgia Tech using Babylon.js. While the focus will be on the value of this approach for remote teaching, it was initially used for face-to-face classes because web-based tools, combined with stand-alone VR displays like the Oculus Quest, support a wider range of student computers and have a much faster development turnaround time compared to traditional game development environments such as Unity and Unreal.
    </p>
    <p>
        The tutorial will be divided into two 90 minutes sessions.
    </p>
    <p>
        <strong>The first session</strong> will be aimed at developers and will introduce the audience to the fundamental concepts, software tools, and workflow for creating immersive virtual reality experiences that run in entirely within a web browser. Specific topics that will be covered include:
    </p>
    <ul>
        <li>Setting up a development environment using Node</li>
        <li>Developing web-based virtual reality experiences using Babylon.js, TypeScript, and WebXR</li>
        <li>Simulating a connected headset and controllers using a WebXR emulator</li>
        <li>Building and deploying experiences to a remote server</li>
        <li>Remotely debugging experiences on the Oculus Quest</li>
    </ul>
    <p>
        This session will be interactive, and template code will be available so that attendees can follow along and replicate the instructors' examples on their own machines. Although this course material was targeted for deployment on the Oculus Quest, the described platform is device agnostic and will work on a range of potential hardware. Access to a headset is also not required, and the tutorial will show how to use an emulator that simulates the presence of a VR device during development.
    </p>

    <p>
        <strong>The second session</strong> will focus primarily on design of an innovative course curriculum for remotely teaching virtual reality and 3D user interface concepts over the web. Although this will be primarily targeted towards educators and students, developers may also find the content useful. Specific topics covered in this session will include:
    </p>
    <ul>
        <li>Practical challenges for remote instruction using VR devices</li>
        <li>Designing learning objectives and content for a web-based 3DUI course</li>
        <li>Using GitHub Classroom to evaluate student code and provide timely feedback</li>
        <li>Facilitating group projects for remote teams</li>
        <li>Incorporating active learning in an online modality</li>
    </ul>
    <p>
        The instructors will also discuss lessons learned from the initial course pilots in Spring and Fall 2020, including things that worked well and areas for improvement. Selected web-based projects from this course will also be demonstrated with permission from the student authors. Finally, research applications, such as conducting remote experiments over the web, will also be discussed.
    </p>

    <h3>Technical Level and Intended Audience</h3>
    <p>
        This tutorial is intended for a wide potential audience in the virtual reality community, and would be technically accessible for students, developers, researchers, and educators. Although basic familiarity with virtual reality hardware and software will be expected, no prior knowledge of web development (e.g., JavaScript or TypeScript) will be assumed.
    </p>

    <h3>Expected Value to Audience</h3>
    <p>
        Web-based game engines and APIs for VR devices (e.g., WebXR) are still very new. These tools are still being actively developed, and online documentation and tutorials are relatively sparse compared to more established professional game development platforms. At the same time, the tools to use them for teaching VR/AR development and 3D user interface concepts are free and relatively lightweight, making them more accessible to a wide range of schools and students. Additionally, the COVID-19 pandemic has fore fronted the unique challenges for remote development and teaching using virtual reality technologies. This tutorial aims to provide value to conference attendees by showing how to leverage an emerging web-based virtual reality software platform and disseminating knowledge from successful remote courses using the Oculus Quest.
    </p>

    {% endif %}
    {% endfor %}
</div>

<div>
    {% for tutorial in site.data.tutorials %}
    {% if tutorial.id == 'T2' %}
    <h2 id="{{ tutorial.id }}">{{ tutorial.title}}</h2>

    <p>
        <strong>Organizers</strong>
    </p>
    <p>
        J. Edward Swan II, Mississippi State University, swan[at]acm.org<br />
        Mohammed Safayet Arefin, Mississippi State University, arefin[at]acm.org<br />
    </p>
    <p>
    <strong style="font-size: 0.8em;color: black"> {{ tutorial.schedule1 }}, {{ tutorial.timezone1 }}</strong>
    </p>
    <p>
        This tutorial will first discuss the replication crisis in empirical science. This term was coined to  describe recent significant failures to replicate empirical findings, in a number of fields, including  medicine and psychology. In many cases, over 50% of previously reported results could not be replicated.  This fact has shaken the foundations of these fields: Can empirical results really be  believed? Should, for example, medical decisions really be based on empirical research? How many psychological findings can we believe?
    </p>
    <p>
        After describing the crisis, the tutorial will revisit enough of the basics of empirical science to explain the origins of the replication crisis. The key issue is that hypothesis testing, which in empirical science is used to establish truth, is the result of a probabilistic process.  However, the human mind is wired to reason absolutely: Humans have a difficult time understanding probabilistic reasoning.  The tutorial will discuss some of the ways that funding agencies, such as the US National Institutes of Health (NIH), have responded to the replication crisis, by, for  example, funding replication studies, and requiring that grant recipients publicly post anonymized  data.  Other professional organizations, including IEEE, have recently begun efforts to enhance the replicability of published research.  In addition, this tutorial will discuss the replication  scenario in different research domains including cognitive psychology, human computer interaction and human factor.
    </p>
    <p>
        Finally, the tutorial will consider how the Virtual Environments community might respond to the replication crisis. In particular, in our community the reviewing process often considers work that involves systems, architectures, or algorithms.  In these cases, the reasoning behind the correctness of the results is usually absolute. Therefore, the standard for accepting papers is that the finding exhibits novelty—to some degree, the result should be surprising. However, this standard does not work for empirical studies, which typically involve human experimental subjects.  Because empirical reasoning is probabilistic, important results need to be replicated, sometimes multiple times, and by different laboratories.  As the replications mount, the field is justified in embracing increasing belief in the results.  In other words, consider a field that, in order to accept a paper reporting empirical results, always requires surprise: This is a field that will not progress in empirical knowledge.
    </p>
    <p>
        The tutorial will end with a call for the community to be more accepting of replication studies. In addition, the tutorial will consider whether actions taken by other fields, in response to the replication crisis, might also be recommendable for the Mixed Reality community.
    </p>
    
    <h3>Technical level, intended audience </h3>
    <p>
        Because of the coverage of statistical material, attendees who have some previous training in statistics might be better able to follow those parts of the tutorial. However, the material is presented at a very high level, with an emphasis on the logical reasoning behind hypothesis testing and probabilistic reasoning. Therefore, we believe that nearly all VR attendees could follow the presentation. 

    </p>
    
    
</div>

<div>
    {% for tutorial in site.data.tutorials %}
    {% if tutorial.id == 'T2' %}
    <h2 id="{{ tutorial.id }}">{{ tutorial.title}}</h2>

    <p>
        <strong>Organizers</strong>
    </p>
    <p>
        J. Edward Swan II, Mississippi State University, swan[at]acm.org<br />
        Mohammed Safayet Arefin, Mississippi State University, arefin[at]acm.org<br />
    </p>
    <p>
    <strong style="font-size: 0.8em;color: black"> {{ tutorial.schedule1 }}, {{ tutorial.timezone1 }}</strong>
    </p>
    
</div>
