---
layout: ieeevr-default
title: "Virbela Instructions"
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
    
    div {
        text-align: justify;
        text-justify: inter-word;
        }

</style>


<div>
    <h1>Virbela / iLRN Virtual Campus Instructions</h1>

    <p>
        Dear IEEEVR 2021 attendee,
    </p>
    <p>
        This year, we will have the poster, doctoral consortium, demo, 3DUI contest, and video presentations on the iLRN Virtual Campus, the 3D venue for the conference, which runs on the Virbela platform. Below is a quick guide to help you set up and navigate the platform and environment.
    </p>

    <div>

        <h2>Accessing the iLRN Virtual Campus</h2>

        <div class="video-container">
            <iframe src="https://www.youtube.com/embed/Et-8EIRN_mw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>

        <p> <br> <br>
            IEEE VR 2021 will happen on the iLRN Virtual Campus, powered by Virbela. You should have received an email inviting you to access the Campus; you will need to click on the “Accept Invitation” link in that email to finish creating your account and download the software.
        </p>
        
        <p> <b>IMPORTANT:</b> The iLRN Virtual Campus is <b style="font-size: 1em;color: black"> not </b> the same as the Virbela Open Campus application that can be downloaded from Virbela’s website. Please use the link provided in the invitation email to access the correct Campus. The application icon should be labelled “iLRN” and not “Virbela”. </p>
        
        <p> Also, if you already have an account associated with your email address on the iLRN Virtual Campus from a previous visit (e.g., the IEEE ISMAR 2020 conference), you will not receive an email invitation. Simply log in to the Campus to gain access. If you need to re-download the software, you can find it at <a href="https://immersivelrn.org/ilrn-virtual-campus">https://immersivelrn.org/ilrn-virtual-campus</a></p>

        <h3>System Requirements</h3>

        <p>Virbela runs on Windows and Mac computers. (At this time, the iLRN Virtual Campus does not support mobile devices.)  The minimum and recommended requirements are listed below:</p>

        <table class="styled-table" style="font-size: 0.8em;">
            <tr>
                <th>Minimum Windows Requirements</th>
                <th>Minimum Mac Requirements</th>
            </tr>
            <tr>
                <td>Windows 7 SP1+</td>
                <td>Mac OS X 10.11</td>
            </tr>
            <tr>
                <td>CPU: 1.8GHz Intel Core i5 or 2GHz AMD Phenom II</td>
                <td>CPU: 2GHz Intel Core i5</td>
            </tr>
            <tr>
                <td>Memory: 4GB</td>
                <td>Memory: 4GB</td>
            </tr>
            <tr>
                <td>Graphics: Graphics device with DX10 (Shader model 4.0)</td>
                <td>Graphics: Intel HD Graphics 4000</td>
            </tr>
            <tr>
                <td>Storage: 2.5GB</td>
                <td>Storage: 2.5GB</td>
            </tr>

        </table>
        <table class="styled-table" style="font-size: 0.8em;">

            <tr>
                <th>Recommended Windows Requirements</th>
                <th>Recommended Mac Requirements</th>
            </tr>
            <tr>
                <td>Windows 7 SP1+ or newer</td>
                <td>Mac OS X 10.11 or newer</td>
            </tr>
            <tr>
                <td>CPU: 2.5GHz Intel Core i7 or 2.2GHz AMD A8</td>
                <td>CPU: 2.5GHz Intel Core i7</td>
            </tr>
            <tr>
                <td>Memory: 8GB</td>
                <td>Memory: 8GB</td>
            </tr>
            <tr>
                <td>Graphics: Dedicated graphics device with DX11 (shader model 4.0) and at least 1GB of on-board memory</td>
                <td>Graphics: GeForce GT 750M or better</td>
            </tr>
            <tr>
                <td>Storage: 2.5GB</td>
                <td>Storage: 2.5GB</td>
            </tr>

        </table>

        <p>
            It is also recommended to use:
        </p>
        <ul>
            <li>Headphones with a built-in microphone</li>
            <li>Power cord plugged in for extended use</li>
        </ul>

        <h3>VR Headsets</h3>

        <p>
            As of today, Virbela supports only tethered headsets, namely Oculus Rift, HTC Vive, and Oculus Quest (both 1 and 2) with a Link cable. Some users have also reported success using Windows Mixed Reality headsets with the platform.
        </p>

        <h3>Installing on Windows</h3>

        <p>
            After downloading the virtual campus, double click the executable file and follow the instructions. Depending on your security settings, your computer may generate a popup that says the app was blocked from opening. Click “Run
        </p>

        <h3>Installing on Mac-OS X</h3>

        <p>
            After downloading the virtual campus, double click the dmg file and then drag the VirBELA iLRN Virtual Campus icon into the Applications folder. When opening VirBELA the application for the first time, the system will ask you if you are sure you want to open it. Click “Open”.
        </p>

    </div>

    <div>

        <h2>Configuring Virbela</h2>

        <p>
            Once you open the iLRN Virtual Campus application, it will download and install the virtual assets for IEEE VR 2021. This may take a while for the first time.
        </p>

        <p>
            <strong>Note:</strong> If the iLRN Virtual Campus application failed to properly install or run, you may need to do a clean install. On Windows, re-run the installer and make sure you check the box labeled "Remove any existing downloads and caches". On Mac, before you reinstall, in the Finder, click on <i> Go > Go to folder </i> and type in <b style="font-size: 1em;color: black">~/Library</b> . Search through the folders and delete any folder that begins with “Virbela” or “iLRN”.
        </p>
            If the problem persists, you can contact Virbela technical support at help[at]virbela.com. (For issues specific to the iLRN Virtual Campus, please email campussupport[at]immersivelrn.org .)
        <p>
            
        </p>

        <p>
            For Windows users, once you open the virtual campus, you can configure some aspects before clicking the “Play!” button to launch the iLRN Virtual Campus.
        </p>

        <!--    image here <img style="width: 20%;" src="/2021/assets/images/sponsors/Virbela-logo.png" alt="Virbela Logo"> -->
        <img src="/2021/assets/images/Images_IEEEVR/image1.png" alt="Play!Button">

        <ul>
            <li>You can change the resolution or graphics quality at this point to reduce the load on your graphics device, which will help Virbela run more smoothly.</li>
            <li>Select “Windowed” if you don’t want Virbela to take up your whole screen.</li>
            <li>Try the “Best” graphics quality, but if you notice stuttering or other performance issues, try one of the lower settings.</li>
        </ul>

        <p>
            If you Accepted the email invitation that was sent to you, you should not need to use the registration feature on the login screen of the iLRN Virtual Campus application. However, if you did not receive the email (make sure you check your spam!), you can attempt to register yourself, but you must <b style="font-size: 1em;color: black"> make sure you use the same email address </b> you used to register IEEE VR 2021. (Otherwise, upon entry to the Virutal Campus you will not have access to the rooms/spaces designated for the conference.). You will also be prompted to enter other information, including your name and organization (or institution). Following registration, you will be automatically redirected to the login screen where you can login with your new account.
        </p>

        <!--    image here -->
        <img src="/2021/assets/images/Images_IEEEVR/image2.png" alt="Registration">

        <h3>Creating your Avatar</h3>

        <p>
            When you log in the first time, you will be taken to the character creation screen. Here you will be able to create your own avatar. This is how the other participants will see you, so you can be creative and have great fun setting up your avatar. Feel free to experiment because you can change it at any time using the <strong>GO TO</strong> menu.
        </p>

        <!--    image here -->
        <img src="/2021/assets/images/Images_IEEEVR/image3.png" alt="Avatar Menu">

        <p>
            After customizing your avatar using the menu (1), select save and exit using the green button in the bottom <b style="font-size: 1em;color: black">right hand </b> corner of the character creation screen (2). This will then bring you into the virtual campus.
        </p>

    </div>

    <div>

        <h3>Using Virbela</h3>

        <p>Once inside the iLRN Virtual Campus, you can explore the campus environment and interact with other IEEE VR 2021 attendees.</p>

        <h2>Walking Around</h2>
        <p>By default, you can move around using the keyboard:</p>

        <table class="styled-table2" style="font-size: 0.8em;">
            <tr>
                <td><strong style="font-size: 1em;color: black">W</strong> or ↑ </td>
                <td>Forward</td>
            </tr>
            <tr>
                <td><strong style="font-size: 1em;color: black">S</strong> or ↓ </td>
                <td>Backward</td>
            </tr>
            <tr>
                <td><strong style="font-size: 1em;color: black">D</strong> or → </td>
                <td>Turn Right</td>
            </tr>
            <tr>
                <td><strong style="font-size: 1em;color: black">A</strong> or ← </td>
                <td>Turn Left</td>
            </tr>
            <tr>
                <td><strong style="font-size: 1em;color: black">Shift</strong></td>
                <td>Run</td>
            </tr>

        </table>

        <p>You can also use your mouse and right-click on the place you want to go and your avatar will walk there.</p>

        <h3>Looking Around</h3>

        <p>By pressing the spacebar, you can unlock your camera and look around freely. Pressing the spacebar again will lock the camera back in place. This function works both when standing and when sitting.</p>

        <h3>Talking with People</h3>

        <p>There are two main ways of communicating within Virbela and you can find them in the lower left of the screen.</p>

        <h4><i>Voice Communication</i></h4>

        <p>This is the primary way to communicate in Virbela. When you arrive in the virtual campus, your microphone will be on mute. It is advised to always keep it on mute when you are not talking to avoid background noise. To speak, you can click at the microphone icon to turn it on. Clicking it again and you will turn it off. You can also talk by pressing and holding the key 1 if you do not want your microphone on all the time.</p>

        <!--    image here -->
        <img src="/2021/assets/images/Images_IEEEVR/image4.png" alt="Voice Communication">

        <p>When you are speaking, a chat bubble will appear both above your head and above the icon. You can only communicate with users who are in the same location as you. For example, if you’re in the Main Stage and someone else is in the Landing Zone, you will not be able to hear each other. Also, you can only hear and talk with people close to you when in open spaces because the audio is spatial in open places. Inside a room, on the other hand, you can hear and talk with anyone regardless of the distance.</p>

        <h4><i>Voice Communication</i></h4>

        <p>The other method of communication is using the chat box. It is next to the microphone icon and you can use it to send messages, share files, communicate with others privately, and see previously sent messages in the room’s chat log. To use the chat, compose your message then click send or press enter on your keyboard. The smiley face provides emojis for adding flair to your messages. To upload a file, click the up arrow on the right side of the chat box.</p>

        <h3>GO TO Menu</h3>

        <p>In the upper left corner of the screen sits the context menu. Here you will find information about how many users are in the same area as you, names of people in the area, and the GO TO menu, which allows you to navigate the world easily.</p>

        <!--    image here -->
        <img src="/2021/assets/images/Images_IEEEVR/image5.png" alt="GO TO Menu">

        <p>The GO TO menu within the context menu allows you to jump to different locations. For example, if you are in the Landing Zone and want to go to the Main Stage for the technical sessions, you would: Select <i>GO TO > Main Stage</i>. Your avatar will then be transported and arrive in the Main Stage.</p>

        <h3>Your Name Menu</h3>

        <p>Below the GO TO Menu, you can see your name, which also reviews a menu that allows you to change your avatar, view your profile and use emotes and actions, such as greeting, clap and dance. You can also trigger them using the keys <strong>F1</strong> to <strong>F8</strong>.</p>

        <!--    image here -->
        <img src="/2021/assets/images/Images_IEEEVR/image6.png" alt="Your Name">

        <h3>Gear Menu</h3>

        <p>The gear menu is in the top right corner and it houses important tools. For instance, <i>Change Avatar</i> allows you to customize your avatar, <i>Find Users</i> helps you locate other people within the virtual campus. Enter the person’s name or display name and it will show you where they are located, and <i>Reinitialize Voice</i> resets your microphone if you’re having issues with feedback on your voice.</p>

        <h4><i>Mic Settings</i></h4>

        <p>This option helps you to make sure the microphone you want to use is selected. You can click on “Windows/Mac Sound Settings” to see how the sound settings are configured on your computer. Higher sensitivity lets in more noise and allows you to speak more quietly. Lower sensitivity lets in less noise and is recommended for loud areas with lots of background noise.</p>


    </div>

    <div>

        <h2>Event etiquette</h2>

        <p>We cannot wait to see you at IEEE VR 2021, but we ask you to pay special attention to the event etiquette below:</p>

        <ul>
            <li>Stay muted on arrival and only open your microphone when you are speaking.</li>
            <li>Do not say or do anything in the virtual campus that you would not do in person.</li>
        </ul>

    </div>
    
    
    <div>
        <h2 id="map">Campus Map</h2>
        <img src="/2021/assets/virbela/iLRN_Virtual_Campus_Map_-_IEEE_VR_2021.jpg" style="width: 100%;" alt="Virbela Virtual Environment map">
        <br/>
        <div style="">
        <center>
            <p style="font-size: 20px;">
                <a href="/2021/assets/virbela/iLRN_Virtual_Campus_Map_-_IEEE_VR_2021.pdf" class="btn btn--primary" style="" download>Download Map as PDF</a>
            </p>
        </center>
    </div>
    </div>
    

    <div>

        <h2>FAQs</h2>

        <p><b style="font-size: 1em;color: black">I’m in the virtual campus, however I am having issues with sound and talking?</b><br>
            Once you are in the iLRN Virtual Campus, student volunteers and iLRN support staff will be available to assist you with troubleshooting sound and other technical issues. If you are having difficulty getting into the iLRN Virtual Campus, please reach out to the IEEE VR 2021 helpdesk on Discord. </p>

        <p><b style="font-size: 1em;color: black">I’m hearing background/environment sounds (e.g., footsteps, birds chirping) but cannot hear other people talking, what should I do?</b><br>
            This is a common issue on Windows computers. To solve this problem open your <i>Control Panel > Hardware and Sounds > Manage Audio devices</i> and select your headphone/speaker as your default device selecting it and clicking on <i>Set Default</i> option. Detailed instructions can be found <a href="https://support.virbela.com/portal/en/kb/articles/can-hear-ambient-noise-but-not-voice-windows"><strong>here</strong></a></p>

        <p><b style="font-size: 1em;color: black">I can hear a lot of people talking, what shall I do?</b><br>
            Many parts of the iLRN Virtual Campus are configured with spatial audio, meaning that like in a real-life event, if you are standing in a busy space with lots of people talking, it’s going to be noisy! Like in real life, if you move away from crowds of people the sound will get quieter. You can also look for private volumes (areas marked by either a dotted blue line or a glowing blue outline); when you step into a private volume, only users within the same private volume will be able to hear one another.</p>

        <p><b style="font-size: 1em;color: black">I keep getting feedback</b><br>
            If you are experiencing feedback, mute your microphone and hold down number 1 when you wish to speak. (This is the push-to-talk function, which works somewhat like a walkie-talkie.)</p>

        <p><b style="font-size: 1em;color: black">I am lost and don’t know how to get back to where I need to be</b><br>
            The iLRN Virtual Campus is a large place, however if you ever find you don’t know where you are. Use your GO TO menu to navigate back to Campus. From Campus you can then use the GO TO to get to any location on the Campus.</p>

        <p><b style="font-size: 1em;color: black">Virbela seems to be running slowly</b><br>
            We recommend shutting down all other applications on your computer while running Virbela to allow the application to run at full speed. Please also see the minimum and recommended hardware specifications listed above. <a href="https://support.virbela.com/portal/en/kb/articles/virbela-is-running-slowly"><strong>This article</strong></a> also contains some additional tips you can try to help alleviate performance issues.</p>

    </div>

</div>
