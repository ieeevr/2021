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
            <td style="font-size: 0.875em;"><a href="#{{ panel.id }}">{{ panel.name }}: {{ panel.title }}</a></td>
        </tr>
        {% endfor %}
    </table>
</div>

<div>
    {% for panel in site.data.panels %}
    {% if panel.id == 'P1' %}
    <h2 id="{{ panel.id }}">Panel: {{ panel.title}}</h2>
    <p style="font-size: 0.8em;">{{ panel.day }}</p>
    
    
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
