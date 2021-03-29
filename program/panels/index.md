---
layout: ieeevr-default
title: "Panels"
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
            <th>Panels</th>
        </tr>
        {% for panel in site.data.panels %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ panel.id }}">{{ panel.title }}</a></td>
        </tr>
        {% endfor %}
    </table>
</div>

<div>
    {% for panel in site.data.panels %}
    {% if panel.id == 'P1' %}
    <h2 id="{{ panel.id }}">Panel: {{ panel.title}}</h2>
    
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == panel.id %}
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
    
    
    <p style="font-size: 0.8em;">{{ panel.day }}, {{panel.start}}, {{ panel.timezone }}</p>
    
    
    <h3 style="color: #00aeef;">Description</h3>
    <p>
        Research on the existence and nature of implicit bias has generated a significant amount of attention in psychology and other social sciences over the past few decades. Considerable scientific and policy interest in prejudice reduction and bias interventions date all the way back to such classic texts as Gordon Allport’s The Nature of Prejudice (1954), where intergroup contact theory as an approach to prejudice reduction was first introduced.  Thousands of hours and millions of dollars have been invested developing and implementing a wide variety of anti-discrimination and anti-bias training programs in different organizational and educational contexts. The efficacy of these efforts, and the conditions under which they are effective and for how long, continues to be an issue at the forefront of research on bias mitigation.
    </p>
    <p>
        This panel assembles a diverse group of experts to discuss the opportunities and challenges in designing, developing, deploying, and assessing the effectiveness of VR-based interventions as a relatively new and novel approach to addressing implicit bias and related constructs including racial empathy and structural competence.
    </p>
    
    <h3 style="color: #00aeef;">Moderator</h3>
    <p>
        <strong style="color: black">Victoria Interrante, Computer Science and Engineering, University of Minnesota, [interran@umn.edu]</strong>
    </p>
    <p>
        Dr. Interrante is a Full Professor in the Department of Computer Science and Director of the university-wide Center for Cognitive Sciences at the University of Minnesota.  Her research focuses on applying insights from visual perception and cognition to the development of more effective virtual reality experiences and the more effective communication of complex information through visual imagery. She enjoys collaborating with colleagues in a wide variety of fields, from architectural design to engineering and medicine.
    </p>
    
    <h3 style="color: #00aeef;">Panelists</h3>
    <p>
        <strong style="color: black">Eugene Borgida, Professor of Psychology and Law at the University of Minnesota, [borgi001@umn.edu]</strong>
    </p>
    <p>
        Dr. Borgida is a Professor of Psychology & Law at the University of Minnesota and a Morse-Alumni Distinguished Professor of Psychology. He is a Fellow of the AAAS (American Association for the Advancement of Science), a Fellow of the APS (Association for Psychological Science), and a Fellow in several divisions of the APA (American Psychological Association). His research interests span social psychology, psychology and law, and political psychology. Dr. Borgida has written on and taught the science of implicit bias, and serves as an expert witness in race and sex discrimination cases. He has presented on the current state of psychological science on implicit racial bias as well as research on the efficacy of bias interventions to the Minnesota Advisory Committee of the U.S. Commission on Civil Rights, and twice has been invited to present this body of research to the U.S. Attorney’s Office and federal district court judges in Minneapolis.
    </p>
    <p>
        <strong style="color: black">Amir Berenjian, co-founder of REM5 VR Lab and REM5 for Good, [amir@rem5vr.com]</strong>
    </p>
    <p>
        Amir Berenjian is the co-founder of REM5, a vertically integrated, immersive technology company focused on using virtual reality to impact positive change and social good. Opened in 2017, REM5 operates a 8,000 sq. ft. facility in Minneapolis, MN that is equipped with the latest in VR technology and hosts over 10,000 guests a year. REM5 for Good has facilitated VR-based training in diversity, equity and inclusion for national and multi-national companies including Cargill, General Mills, Target, and Boston Scientific, and has offered VR-based training to local police departments, focusing on showing how implicit bias comes into play in high-stress scenarios and promoting safer, more empathetic interactions. Amir is the lead designer of Steps of Privilege VR, an interactive VR experience that provides a safe space for users to explore and reflect on the nuances of their own privilege. Prior to co-founding REM5, he spent 12+ years in investment banking and corporate finance. Amir is a 2020 Oculus Launch Pad Fellow.
    </p>
    <p>
        <strong style="color: black">Courtney D. Cogburn, Associate Professor of Social Work, Columbia University, [cc3803@columbia.edu]</strong>
    </p>
    <p>
        Dr. Cogburn is the lead creator of 1000 Cut Journey, an immersive virtual reality racism experience that was developed in collaboration with the Virtual Human Interaction Lab at Stanford University and which premiered at the Tribeca Film Festival in 2018. Her research employs a transdisciplinary strategy to improve the characterization and measurement of racism, and explores the use of emerging technologies, including computational social science to examine patterns and psychosocial effects of cultural racism and how virtual reality experiences can lead to changes in attitudes, social perception and engagement (empathy, racial bias, structural competence and behavior). She received her Ph.D. in Education and Psychology, and MSW from the University of Michigan, and completed postdoctoral training at Harvard University in the Robert Wood Johnson Health & Society Scholar Program and at the Institute for Social Research at the University of Michigan. She is a board member of the the International Center Advocates Against Discrimination, a human rights organization working at the intersection of legal innovation and human centered design.
    </p>
    <p>
        <strong style="color: black">Tabitha Peck, Assistant Professor of Mathematics and Computer Science, Davidson College, [tapeck@davidson.edu]</strong>
    </p>
    <p>
        Dr. Peck is a leading researcher in the IEEE VR community who has, among other work, published extensively on the topic of mitigating implicit bias and stereotype threats using VR technology.  Her 2013 paper “Putting yourself in the skin of a black avatar reduces implicit racial bias” has been cited over 450 times.  Dr. Peck earned her PhD from the University of North Carolina at Chapel Hill and was a postdoctoral researcher in Mel Slater’s EventLab at the University of Barcelona. She received an NSF CAREER award to continue her work investing the potential of VR to mitigate stereotype threats in STEM classrooms.
    </p>
    <p>
        <strong style="color: black">Domna Banakou, Postdoctoral Researcher, Experimental Virtual Environments for Neuroscience and Technology (Event Lab), Universitat de Barcelona, [dbanakou@ub.edu]</strong>
    </p>
    <p>
        Dr. Domna Banakou completed her PhD in Clinical Psychology and Psychobiology at the University of Barcelona in 2017. She also holds a Master’s degree in Computer Graphics, Vision and Imaging from University College London (UCL), UK, and a Bachelor’s degree in Computer Science from the Ionian University, Greece. She combines technical expertise and experience in research methodologies to understand and promote the use of virtual reality in the fields of psychology and cognitive neuroscience. Her research focuses on body representation in immersive virtual reality, exploring the perceptual, behavioral, and higher-level cognitive correlates of body ownership illusions that occur as a function of the type of body in which embodiment occurs. Embodying a different race body and studying implicit bias is of particular interest in her work, where she has previously addressed the longer-term effects of these experiences but also the impact of the social context of the VR scenario on shaping such implicit attitudes.
    </p>    
    
    {% endif %}
    {% endfor %}
</div>


<div>
    {% for panel in site.data.panels %}
    {% if panel.id == 'P2' %}
    <h2 id="{{ panel.id }}">Panel: {{ panel.title}}</h2>
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == panel.id %}
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
    
    <p style="font-size: 0.8em;">{{ panel.day }}, {{panel.start}}, {{ panel.timezone }}</p>
    
    
    <h3 style="color: #00aeef;">Description</h3>
    <p>
        XR is undergoing rapid development at a time of societal transformation. Will the arts be a driving force and determining factor for the future of immersive technologies? Virtual experiences emerged as a primary mode of engaging with each other and the arts in 2020.  Experiencing the world from our homes has compelled us to delve deeper into our humanity and the power of virtual and immersive technology to bridge our physical, social and emotional connections. Artists and technologists are collaborating to create new modalities of expression and societal impact through XR. This panel explores the multiple perspectives of artists, industry, and technologists in shaping the future of XR in the arts, culture and entertainment.
    </p>
    
    <h3 style="color: #00aeef;">Moderator</h3>
    <p>
        <strong style="color: black">Ruth West, Professor, University of North Texas, [Ruth.West@unt.edu]</strong>
    </p>
    <p>
        Ruth West is an artist, professor at University of North Texas and director of the xREZ Art + Science Lab (http://xrezlab.com). Ruth creates social and collaborative data-driven extended reality art and interactive installations. Her work has been presented internationally at venues including MONA FOMA Festival (Museum of Old and New Art), Los Angeles Municipal Art Gallery, FILE 09 Sao Paulo, SIGGRAPH, WIRED Magazine’s NextFest, Perot Museum of Nature and Science, and the UCLA Fowler Museum.
    </p>
    
    <h3 style="color: #00aeef;">Panelists</h3>
    <p>
        <strong style="color: black">Margaret Dolinsky, Associate Professor, Indiana University, [dolinsky@iu.edu]</strong>
    </p>
    <p>
        Margaret Dolinsky is Associate Professor at the Eskenazi School of Art, Architecture+Design at Indiana University. She received an MFA from University of Illinois at Chicago (EVL) and a PhD from University of Plymouth, UK. Dolinsky creates whimsical portraits of people and landscapes for VR, interactive opera and experimental film. Her work has been shown in North and South America, Europe, Asia, and Australia in museums, festivals, and galleries. Dolinsky appears in “New Media Futures: The Rise of Women in the Digital Arts” by Donna Cox, et al. and VR Developer Gems (Sherman, Ed.), Dolinsky co-chairs IS&T Engineering Reality of Virtual Reality conference.  <a href="https://dolinsky.pages.iu.edu/" target="_blank">https://dolinsky.pages.iu.edu/</a>
    </p>
    
    <p>
        <strong style="color: black">Domhnaill Hernon, VP Research and Innovation, Nokia Bell Labs, [domhnaill.hernon@nokia-bell-labs.com]</strong>
    </p>
    <p>
        Domhnaill Hernon is Head of Experiments in Arts and Technology (E.A.T.) at Nokia Bell Labs. He graduated with a B.Eng in Aeronautical Engineering, a Ph.D in fundamental fluid mechanics from the University of Limerick and an Executive M.B.A. from Dublin City University, Ireland. He is passionate about turning research/ideas into reality and exploring the bounds of creativity to push the limits of technology. Domhnaill was previously responsible for turning Bell Labs disruptive research assets into proto-solutions that could be tested at scale in the market, and he established new methods to overcome the “Innovation Valley of Death”. He is currently responsible for Bell Labs global activities in E.A.T. where he collaborates with the artistic and creative community to push the limits of technology to solve the greatest human need challenges. <a href="https://www.bell-labs.com/collaboration-opportunities/eat/" target="_blank">https://www.bell-labs.com/collaboration-opportunities/eat/</a>
    </p>
    <p>
        <strong style="color: black">Savannah Niles, Principal Designer, Magic Leap, [savannahniles@gmail.com]</strong>
    </p>
    <p>
        Savannah Niles is a multi-disciplinary design and technology leader in the spatial computing industry. She's currently Director of Interaction Design and Product Experience at Magic Leap, a Florida-based spatial computing startup with $2.6 billion in funding. For 5 years at Magic Leap, Savannah has designed, prototyped, and shipped a wide range of hardware and software products, with 20+ patent applications and grants. She continues to contribute as a multidisciplinary leader across design, technology, and strategy roles. Currently, Savannah leads interaction design and prototyping for Magic Leap's core hardware and software platforms. Previously, designed interactive experiences for Walt Disney Imagineering and Twitter. MIT Media Lab graduate. Juror at SIGGRAPH. 20+ patent applications and grants. <a href="https://www.savannahniles.com/" target="_blank">https://www.savannahniles.com/</a>
    </p>
    
    <p>
        <strong style="color: black">Kristine Severson, Strategic Partnerships and Content, Video Games, AR/VR and Board of Directors, The Hydrous, [seversonkristine@gmail.com]</strong>
    </p>
    <p>
        Kristine Severson is an AR/VR, video games, digital media, and consumer electronics veteran with expertise in strategic partnerships, business development, content acquisition and licensing, digital distribution and marketing, product and technology evangelism, and publisher and developer relations. Formerly at Sony Playstation / HTC Vive / Rockstar Games, Take Two Interactive / 2K Games. <a href="http://www.vrforimpact.com " target="_blank">http://www.vrforimpact.com </a>
    </p>

    <p>
        <strong style="color: black">Nicola Triscott, Director/CEO, FACT, [nicola.triscott@fact.co.uk]</strong>
    </p>
    <p>
        Nicola Triscott PhD is a curator, researcher and writer, specializing in the intersections between art, science, technology and society. Since 2019, Nicola has been Director/CEO of FACT (Centre for Film, Art & Creative Technology) in Liverpool, UK, where she curated the exhibition And Say the Animal Responded? in 2020. Previously, she was the founding Artistic Director/CEO of Arts Catalyst (from 1994 to 2019) and Principal Research Fellow at University of Westminster (2017-19). Over 25 years, Nicola built Arts Catalyst into one of the UK’s most distinctive and respected art and research organisations, distinguished by ambitious artists’ commissions, including notable projects by Tomás Saraceno, Otolith Group, Ashok Sukumaran, Marko Peljhan, Ariel Guzik, and Critical Art Ensemble. Nicola lectures and publishes internationally. <a href="https://nicolatriscott.org/" target="_blank">https://nicolatriscott.org/</a>
    </p>
    
        {% endif %}
    {% endfor %}
</div>

<div>
    {% for panel in site.data.panels %}
    {% if panel.id == 'P3' %}
    <h2 id="{{ panel.id }}">Panel: {{ panel.title}}</h2>
    
    <!-- TAKE ME TO THE EVENT START -->
    {% for event in site.data.events %}
    {% if event.id == panel.id %}
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
    
    <p style="font-size: 0.8em;">{{ panel.day }}, {{panel.start}}, {{ panel.timezone }}</p>
    
    
    <h3 style="color: #00aeef;">Description</h3>
    <p>
        Humans are social beings, and even in VR we typically do not want to be alone. As VR becomes increasingly utilized for a wide range of applications, virtual humans are expected to play increasingly important roles.  A lot of research has concentrated on making virtual humans look and move photo-realistically. Here we argue that the fundamental question is what makes virtual humans effective, in the sense that people respond to them in a way that is useful for and predicted by the application. For example, if the purpose of the application is to make people laugh, then no matter how photorealistic or how expressive the virtual humans involved might be, if the human participants do not laugh then the application would have failed. So, the question shifts from ‘How realistic can we make these virtual humans’ to ‘How should the virtual humans look and behave in order to make you laugh as a human comedian would’ - which may not require high levels of animation realism and photorealism.
    </p>
    <p>
        In this panel, we will discuss the theoretical background behind how effective responses might be elicited by virtual humans and the methodologies used to measure the impact they have on participants. We suggest that in VR the most important question about a virtual human is not: “does it look real”, but “do participants respond to it as if it were a real human”. For example, does the virtual psychotherapist contribute to your wellbeing? This shifts the focus from issues intensively studied in the computer graphics and animation communities to questions that are unique to VR. 
    </p>
    <p>
        We will discuss how eliciting realistic responses is related to all levels of virtual human design and development:
    </p>
    <ul>
        <li>With respect to appearance, are there some factors more important than others in order to elicit realistic responses?</li>
        <li>In terms of character animation, what are the key features required of a virtual human to be plausible and thus trigger more realistic responses?</li> 
        <li>When it comes to multimodal integrated behavior, such as combined gesture, speech, and facial expression -- what are the key factors that could help maintain consistency? </li>
        <li>Because VR is interactive, virtual humans have to be responsive to user inputs in real-time. However, human inputs are rich and sometimes very subtle. What is the best practice here?</li>
        <li>One of the key application areas for virtual humans is training. For instance, medical students could be routinely spending 1-2 hours with virtual patients to practise their consultation skills. In this situation, the question is: how do you get humans to want to spend time with virtual humans? How does one frame interactions with virtual humans so people know how and why they should interact with them?</li>
    </ul>
    <p>
        Finally, as our essential question for any VR application involving virtual humans is: “do participants respond to them as if they were real?” We will wrap up our discussion with the following:
    </p>
    <ul>
        <li>Give one example of a novel measurement you used that provides convincing evidence that participants did respond towards it as if it were real.</li>
    </ul>
    
    
    <h3 style="color: #00aeef;">Moderator</h3>
    <p>
        <strong style="color: black">Xueni Pan, Department of Computing, Goldsmiths, University of London, UK [x.pan@gold.ac.uk]</strong>
    </p>
    <p>
        Xueni Pan is an Assistant Prof. in VR in Virtual Reality at Goldsmiths College, University of London. She worked at UCL in both Computer Science and Institute of Cognitive Neuroscience. Dr Pan has a unique interdisciplinary research profile, with journal and conference publications on both VR technology and social neuroscience. Her work has featured on the BBC, in New Scientist magazine and the Wall Street Journal. Her Coursera VR specialisation has attracted over 80,000 registered learners globally, and she co-leads on the MA/MSc in Virtual and Augmented Reality at Goldsmith’s Computing.
    </p>
    
    <h3 style="color: #00aeef;">Panelists</h3>
    <p>
        <strong style="color: black">Doron Friedman, Sammy Ofer School of Communications, Israel [doronf@idc.ac.il]</strong>
    </p>
    <p>
        Doron Friedman an Associate Prof. in the Sammy Ofer School of Communications and the head of the Advanced Reality Lab (https://arlidc.ac.il), Israel. Since 2008, Prof. Friedman and his lab members have been involved in several national and international projects in the areas of telepresence, VR, and advanced human computer interfaces. Doron's research is highly multidisciplinary and has been published in top scientific journals and peer reviewed conferences, including Artificial Intelligence, Human Computer Interaction, Journal of Neural Engineering, Journal of Neuroscience, PNAS, and more. Friedman and his lab members also frequently take part in real world industry projects.
    </p>
    <p>
        <strong style="color: black">Benjamin Lok, Computer and Information Sciences and Engineering Department, University of Florida, USA [lok@cise.ufl.edu] 
</strong>
    </p>
    <p>
        Ben Lok is a Professor in the Computer and Information Sciences and Engineering Department at the University of Florida and entrepreneur, having previously co-founded Shadow Health. Shadow Health’s virtual humans are used by half of all nursing students and impacts nearly every person in the US and Canada. Professor Lok's research focuses on using virtual humans and mixed reality to train communication skills within the areas of virtual environments, human-computer interaction, and computer graphics. He was awarded the 2019 UF Innovator of the Year and multiple best paper awards involving virtual human research.
    </p>
    <p>
        <strong style="color: black">Mel Slater, Event Lab, University of Barcelona, Spain [melslater@ub.edu]
</strong>
    </p>
    <p>
        Mel Slater is co-Director of the Event Lab at the University of Barcelona. He was previously Professor of Virtual Environments at University College London. He has been involved in research in virtual reality since the early 1990s and has been the first supervisor of more than 40 students who achieved their PhDs in graphics and virtual reality since 1989. He was awarded the 2005 IEEE Virtual Reality Career Award: ‘In Recognition of Pioneering Achievements in Theory and Applications of Virtual Reality’. He is Field Editor of Frontiers in Virtual Reality. He is co-founder of Virtual Bodyworks.
    </p>

        {% endif %}
    {% endfor %}
</div>


