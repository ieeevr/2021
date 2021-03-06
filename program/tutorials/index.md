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
        This tutorial will first discuss the replication crisis in empirical science. This term was coined to describe recent significant failures to replicate empirical findings, in a number of fields, including medicine and psychology. In many cases, over 50% of previously reported results could not be replicated. This fact has shaken the foundations of these fields: Can empirical results really be believed? Should, for example, medical decisions really be based on empirical research? How many psychological findings can we believe?
    </p>
    <p>
        After describing the crisis, the tutorial will revisit enough of the basics of empirical science to explain the origins of the replication crisis. The key issue is that hypothesis testing, which in empirical science is used to establish truth, is the result of a probabilistic process. However, the human mind is wired to reason absolutely: Humans have a difficult time understanding probabilistic reasoning. The tutorial will discuss some of the ways that funding agencies, such as the US National Institutes of Health (NIH), have responded to the replication crisis, by, for example, funding replication studies, and requiring that grant recipients publicly post anonymized data. Other professional organizations, including IEEE, have recently begun efforts to enhance the replicability of published research. In addition, this tutorial will discuss the replication scenario in different research domains including cognitive psychology, human computer interaction and human factor.
    </p>
    <p>
        Finally, the tutorial will consider how the Virtual Environments community might respond to the replication crisis. In particular, in our community the reviewing process often considers work that involves systems, architectures, or algorithms. In these cases, the reasoning behind the correctness of the results is usually absolute. Therefore, the standard for accepting papers is that the finding exhibits novelty—to some degree, the result should be surprising. However, this standard does not work for empirical studies, which typically involve human experimental subjects. Because empirical reasoning is probabilistic, important results need to be replicated, sometimes multiple times, and by different laboratories. As the replications mount, the field is justified in embracing increasing belief in the results. In other words, consider a field that, in order to accept a paper reporting empirical results, always requires surprise: This is a field that will not progress in empirical knowledge.
    </p>
    <p>
        The tutorial will end with a call for the community to be more accepting of replication studies. In addition, the tutorial will consider whether actions taken by other fields, in response to the replication crisis, might also be recommendable for the Mixed Reality community.
    </p>

    <h3>Technical level, intended audience </h3>
    <p>
        Because of the coverage of statistical material, attendees who have some previous training in statistics might be better able to follow those parts of the tutorial. However, the material is presented at a very high level, with an emphasis on the logical reasoning behind hypothesis testing and probabilistic reasoning. Therefore, we believe that nearly all VR attendees could follow the presentation.

    </p>

        {% endif %}
    {% endfor %}

</div>

<div>
    {% for tutorial in site.data.tutorials %}
    {% if tutorial.id == 'T3' %}
    <h2 id="{{ tutorial.id }}">{{ tutorial.title}}</h2>

    <p>
        <strong>Organizers</strong>
    </p>
    <p>
        Adam O. Bebko, Biomotionlab, York University, adambebko[at]gmail.com<br />
        Anne Thaler, Biomotionlab, York University, athaler[at]yorku.ca<br />
    </p>
    <p>
        <strong style="font-size: 0.8em;color: black"> {{ tutorial.schedule1 }}, {{ tutorial.timezone1 }}</strong>
    </p>

    <p>
        Advances in virtual reality (VR) technology have provided a wealth of valuable new approaches to researchers. Coding VR experiments from scratch is technically challenging. Therefore, researchers typically use software such as Unity game engine to create and edit virtual scenes that interface with VR displays. However, Unity lacks built-in tools for controlling experiments, and existing third -party add-ins require substantial scripting and coding knowledge to design even the simplest of experiments, especially for multifactorial designs.
    </p>
    <p>
        In this tutorial, we will provide a brief overview of a free and open-source tool called the BiomotionLab Toolkit for Unity Experiments (bmlTUX): https://biomotionlab.github.io/TUX/. Unlike existing tools, bmlTUX provides a graphical interface for configuring factorial experimental designs and turning them into executable experiments. New experiments work “out-of-the-box” and can be created with fewer than twenty lines of code. The toolkit can automatically handle the combinatorics of both random and counterbalanced factors, mixed designs with within and between-subject factors, and blocking, repetition, and randomization of trial order.
    </p>
    <p>
        During runtime, the experimenter can interactively control the flow of trials and monitor the progression of the experiment. Despite its simplicity, bmlTUX remains highly flexible and customizable, catering to both novice and advanced coders. The toolkit simplifies the process of getting experiments up and running quickly without the hassle of complicated scripting. The toolkit interfaces seamlessly with VR and AR packages, allowing for quick implementation of mixed reality experiments in Unity.
    </p>

    <h3>Technical level and intended audience</h3>
    <p>
        Users should already have the latest version of Unity installed and be familiar with basic controls (Scene view, Game view, Inspectors, how to add scripts to GameObjects). Unity Editor version 2020.1 or above will be suitable. Users should also have some basic C# coding knowledge. We will target the novice-level coder by explaining all steps. However, some basic C# experience will be essential to follow along.
    </p>

    <h3>Expected value to that audience</h3>
    <p>
        Attendees will learn how to design and set up a new VR-compatible behavioural experiments using bmlTUX. This should help attendees accelerate their workflows to create VR experiments, and greatly reduce the amount of coding required to get up and running. This tutorial will also familiarize users with implementing third-party packages into Unity Game Engine.
    </p>

        {% endif %}
    {% endfor %}
    
</div>

<div>
    {% for tutorial in site.data.tutorials %}
    {% if tutorial.id == 'T4' %}
    <h2 id="{{ tutorial.id }}">{{ tutorial.title}}</h2>

    <p>
        <strong>Organizers</strong>
    </p>
    <p>
        Mirjam Vosmeer, Amsterdam University of Applied Sciences, m.s.vosmeer[at]hva.nl<br />
        Christian Roth, Utrecht University of the Arts, christian.roth[at]hku.nl<br />
    </p>
    <p>
        <strong style="font-size: 0.8em;color: black"> {{ tutorial.schedule1 }}, {{ tutorial.timezone1 }}</strong>
    </p>

    <p>
        This tutorial will start by giving a general overview of research into storytelling for VR and about the field of interactive narrative design, presenting a number of cases studies and discussing ways to connect research with questions gained from the industry. The concept of interaction will be presented as a tool for storytelling, as well as the concept of Meaningful VR. A short overview of how VR producers have used the medium in attempts to change viewers’ attitudes and values, often by enabling them to enter another person’s body or experience a slice of another’s life is given. In this context a number of earlier initiatives such as VR for Good and VR for Impact will be presented.
    </p>
    <p>
        After this introduction a range of related theoretical concepts, such as embodiment, acknowledgment, positive technology, media-effects, parasocial interaction, and ludonarrative meaning-making will be discussed, also addressing how technological developments have enabled new ways of including interaction in VR. Subsequently, a conceptual model that aims to bring together different concepts of interaction in VR will be presented: this model can be used to differentiate between narrative and physical interaction, which can be either active or passive.
    </p>
    <p>
        In the following interactive part of the tutorial, participants will be asked to take half an hour offline to look into a VR experience or a 360° video of their choice, and use the conceptual model to interpret the observed interactive elements. After this break, participants will be asked to present and discuss their findings with the group.
    </p>
    <p>
        In the last part of the tutorial, the research project VR for Diversity that was started in October 2020 will be presented, aiming to connect insights that have been gained in the previous part of the tutorial to explore the groups ideas on how interaction design can be applied to realize a Meaningful VR installation that will challenge viewers to (re)consider their views, beliefs and/or opinions on the topic of diversity.
    </p>

    <h3>Technical level, intended audience and value </h3>
    <p>
        The intended audience of this tutorial is interested in the possibilities of VR as a meaningful storytelling medium that can evoke positive change and create new insights with a transformative potential. Previous experience with different types of VR is helpful, but no technical skills are required.
    </p>
    <p>
        Value lies in the insights into the concept of Meaningful VR from both a psychological and design perspective and the demonstration and discussion of promising applications.
    </p>

        {% endif %}
    {% endfor %}
    
</div>

<div>
    {% for tutorial in site.data.tutorials %}
    {% if tutorial.id == 'T5' %}
    <h2 id="{{ tutorial.id }}">{{ tutorial.title}}</h2>

    <p>
        <strong>Organizers</strong>
    </p>
    <p>
        Darlene Barker, University of Massachusetts Lowell, MA, darlene_barker[at]student.uml.edu<br/>
        Haim Levkowitz, University of Massachusetts Lowell, MA, haim_levkowitz[at]uml.edu<br/>
    </p>
    <p>
        <strong style="font-size: 0.8em;color: black"> {{ tutorial.schedule1 }}, {{ tutorial.timezone1 }}</strong>
    </p>
    
    <p>
        To make more impact on social interaction within virtual reality (VR), we need to consider the impact of emotions on our interpersonal communications and how we can express them within VR. This tutorial will show the introductory research on the topic, where we propose the use of emotions that are based upon the use of voice, facial expressions, and touch to create the emotional closeness and nonverbal intimacy needed in nonphysical interpersonal communication. Virtual and long-distance communications lack the physical contact that we have with in-person interaction as well as the nonverbal cues that enhance what the conversation is conveying. The use of haptic devices and tactile sensations can help with the delivery of touch between parties and machine learning can be used for emotion recognition based on data collected from other sensory devices; all working towards better long-distance communications.
    </p>
    <p>
        In today’s world, we are forced to remain apart due to the global pandemic and the safety measures needed to prevent its spread. So, having a better means of communicating with loved ones would be invaluable. Outside of the pandemic, the ability to experience touch as well as other senses within VR could help enhance communication between family who lives at a distance or family who is separated because some of them must travel for work. Those who are visually impaired may also benefit from such technology.
    </p>
    <p>
        Topics to be covered include the following:
    </p>
    <ul>
        <li>Overview of how emotions are currently being interpreted.</li>
        <li>Overview of the instructors’ implementing of emotions to include touch in VR from a software approach, an initial stage research.</li>
        <li>More detailed approach of the interpretation of nonverbal communication in VR, movement, facial expressions, and touch by the avatar.</li>
        <li>Applications of the use of emotions in VR.</li>
        <li>Discussion of further research in emotions in VR</li>
    </ul>

    <h3>Technical level, intended audience and value </h3>
    <p>
        All can benefit from this. The tutorial will be accessible technically from high-schooler and above.
        Given our current Covid-19 measures, it could add value to communications with family at a distance and close. Outside of that, visually impaired people could benefit from this. Also, long distance communication can benefit from this research.
    </p>

        {% endif %}
    {% endfor %}
    
</div>
