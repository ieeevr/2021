---
layout: ieeevr-default
title: "Venue"
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

</style>


<div>
    <h1>Venue</h1>  
    
    <p>Dear IEEE VR 2021 attendee, it is a pleasure to have you with us in the first IEEE VR 2021 in Virtual Reality ever. Here we have a quick guide to help you set up and make your first steps in the VR platform.</p>
    
    <div>
    
        <h2>Setting up VirBELA</h2>

        <p>IEEE VR 2021 will happen in the iLRN Virtual Campus using VirBELA. To download and install it, use the link we provided in the email sent by the IEEE VR Office about the VR platform.</p>

        <h3>System Requirements</h3>

        <p>VirBELA runs on Windows and Mac computers. The minimum and recommended requirements are listed below:</p>

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

        <p>It is also recommended to use:</p>
        <ul>
            <li>Headphones and a microphone</li>
            <li>Power cord plugged in for extended use</li> 
        </ul>
        
        <h3>VR  Headsets</h3>

        <p>As of today, VirBELA supports Oculus Rift and HTC Vive.</p>

        <h3>Installing on Windows</h3>

        <p>After downloading the virtual campus, double click the executable file and follow the instructions. Depending on your security settings, your computer may generate a popup that says the app was blocked from opening. Click “Run anyway”. If you see “Do you want to allow this app… to make changes to your PC?”, click “Yes”.</p>

        <h3>Installing on Mac OSX</h3>

        <p>After downloading the virtual campus, double click the dmg file and then drag the VirBELA icon into the Applications folder. When opening VirBELA for the first time, the system will ask you if you are sure you want to open it. Click “Open”.</p>
    
    </div>
    
    <div>
        
        <h2>Configuring VirBELA</h2>

            <p>Once you open the iLRN Virtual Campus using VirBELA, it will download and install the virtual assets for IEEE VR 2021. This may take a while for the first time.</p>
        
            <p><b>Note:</b> If VirBELA failed to properly install or run, you may need to remove all previous campuses and do a clean install. If the problem persists, you can contact VirBELA technical support at help@virbela.com.</p>
        
            <p>For Windows users, once you open the virtual campus, you can configure some aspects before clicking the “<b>Play!</b>” button to launch VirBELA.</p>
        
        <!--    image here -->
        <img src="assets\images\Images_IEEEVR\image1.png" alt="Play!Button">

            <ul>
                <li>You can change the resolution or graphics quality at this point to reduce the load on your graphics device, which will help VirBELA run smoother.</li>
                <li>Select “Windowed” if you don’t want VirBELA to take up your whole screen.</li>
                <li>Try the “Best” graphics quality, but if you notice stuttering or other performance issues, try one of the lower settings.</li>
            </ul>
        
            <p>If you do not have an account, you need to register before using the virtual campus for the first time. You will need to provide the same email you used to register IEEE VR 2021 along with other personal information, such as name, organization (or institution), and others. After that, you will be automatically redirected to the login screen where you can login with your new account.</p>
        
        <!--    image here -->
        
            <h3>Creating your Avatar</h3>
        
            <p>When you log in the first time, you will be taken to the character creation screen. Here you will be able to create your own avatar. This is how the other participants will see you, so you can be creative and have great fun setting up your avatar. Feel free to experiment because you can change it at any time using the <strong>GO TO</strong> menu.</p>
        
        <!--    image here -->
        
            <p>After customizing your avatar using the menu (1), select save and exit using the green button in the bottom right hand corner of the character creation screen (2). This will then bring you into the virtual campus.</p>

        </div>
    
    <div>
        
        <h3>Using VirBELA</h3>
        
        <p>Once inside VirBELA, you can explore the virtual campus and interact with other IEEE VR 2021 attendees.</p>
        
        <h2>Walking Around</h2>
        <p>By default, you can move around using the keyboard:</p>
        
        <table class="styled-table" style="font-size: 0.8em;">
            <tr>
                <td><strong>W</strong> or <i class='fas fa-arrow-up'></i> </td>
                <td>Forward</td>
            </tr>
            <tr>
                <td><strong>S</strong> or <i class='fas fa-arrow-down'></i></td>
                <td>Backward</td>
            </tr>
            <tr>
                <td><strong>D</strong> or <i class='fas fa-arrow-right'></i></td>
                <td>Turn Right</td>
            </tr>
            <tr>
                <td><strong>A</strong> or <i class='fas fa-arrow-left'></i></td>
                <td>Turn Left</td>
            </tr>
            <tr>
                <td><strong>Shift</strong></td>
                <td>Run</td>
            </tr>
            
        </table>
        
        <p>You can also use your mouse and right-click on the place you want to go and your avatar will walk there.</p>
        
        <h3>Looking Around</h3>
        
        <p>By pressing the spacebar, you can unlock your camera and look around freely. Pressing the spacebar again will lock the camera back in place. This function works both when standing and when sitting.</p>
        
        <h3>Talking with People</h3>
        
        <p>There are two main ways of communicating within VirBELA and you can find them in the lower left of the screen.</p>
        
        <h4><i>Voice Communication</i></h4>
        
        <p>This is the primary way to communicate in VirBELA. When you arrive in the virtual campus, your microphone will be on mute. It is advised to always keep it on mute when you are not talking to avoid background noise. To speak, you can click at the microphone icon to turn it on. Clicking it again and you will turn it off. You can also talk by pressing and holding the key 1 if you do not want your microphone on all the time.</p>
        
    <!--    image here -->
        
        <p>When you are speaking, a chat bubble will appear both above your head and above the icon. You can only communicate with users who are in the same location as you. For example, if you’re in the Main Stage and someone else is in the Landing Zone, you will not be able to hear each other. Also, you can only hear and talk with people close to you when in open spaces because the audio is spatial in open places. Inside a room, on the other hand, you can hear and talk with anyone regardless of the distance.</p>
        
        <h4><i>Chat Communication</i></h4>
        
        <p>The other method of communication is using the chat box. It is next to the microphone icon and you can use it to send messages, share files, communicate with others privately, and see previously sent messages in the room’s chat log. To use the chat, compose your message then click send or press enter on your keyboard. The smiley face provides emojis for adding flair to your messages. To upload a file, click the up arrow on the right side of the chat box.</p>
        
        <h3>GO TO Menu</h3>
        
        <p>In the upper left corner of the screen sits the context menu. Here you will find information about how many users are in the same area as you, names of people in the area, and the GO TO menu, which allows you to navigate the world easily.</p>
        
        <!--    image here -->
        
        <p>The GO TO menu within the context menu allows you to jump to different locations. For example, if you are in the Landing Zone and want to go to the Main Stage for the technical sessions, you would: Select <i>GO TO > Main Stage</i>. Your avatar will then be transported and arrive in the Main Stage.</p>
        
        <h3>Your Name Menu</h3>
        
        <p>Below the GO TO Menu, you can see your name, which also reviews a menu that allows you to change your avatar, view your profile and use emotes and actions, such as greeting, clap and dance. You can also trigger them using the keys <strong>F1</strong> to <strong>F8</strong>.</p>
        
        <!--    image here -->
        
        <h3>Gear Menu</h3>
        
        <p>The gear menu is in the top right corner and it houses important tools. For instance, <i>Change Avatar</i> allows you to customize your avatar, <i>Find Users</i> helps you locate other people within the virtual campus. Enter the person’s name or display name and it will show you where they are located, and <i>Reinitialize Voice</i> resets your microphone if you’re having issues with feedback on your voice.</p>
        
        <h4><i>Mic Settings</i></h4>
        
        <p>This option helps you to make sure the microphone you want to use is selected. You can click on “Windows/Mac Sound Settings” to see how the sound settings are configured on your computer.  Higher sensitivity lets in more noise and allows you to speak more quietly. Lower sensitivity lets in less noise and is recommended for loud areas with lots of background noise.</p>
        
        
    </div>
    
    <div>
    
        <h2>Event etiquette</h2>
        
        <p>We cannot wait to see you at IEEE VR 2021, but we ask you to pay special attention to the event etiquette below:</p>
        
        <ul>
            <li>Please do not go on any of the stages during sessions unless you are invited. If you do, a student volunteer will remove you from the venue and you will have to re-enter.</li>
            <li>Stay muted on arrival and only open your microphone when you are speaking.</li>
            <li>Do not say or do anything in the virtual campus that you would not do in person.</li>
        </ul>
    
    </div>
    
    <div>
    
        <h2>FAQ</h2>
        
        <p><b style="font-size: 0.8em;color: black">I’m in the virtual campus, however I am having issues with sound and talking?</b></p>
        <p>Any technical issues when you are inside the world, VirBELA Concierge and technical staff will be available on campus to help you with. </p>
        
        <p><b style="font-size: 0.8em;color: black">I’m hearing a background sound but cannot hear people talking, what should I do?</b></p>
        <p>To solve this problem using <i>Windows</i>, open your <i>Control Panel > Hardware and Sounds > Manage Audio devices</i> and select your headphone/speaker as your default device selecting it and clicking on <i>Set Default</i> option. </p>
        
        <p><b style="font-size: 0.8em;color: black">I can hear a lot of people talking, what shall I do?</b></p>
        <p>Like in a real-life event, if you are standing in a busy space with lots of people talking it’s going to be noisy. Like in real-life, if you move away from crowds of people the sound will get quieter.</p>
        
        <p><b style="font-size: 0.8em;color: black">I keep getting feedback</b></p>
        <p>If you are experiencing feedback, turn off your microphone and hold down number 1 when you wish to speak.</p>
        
        <p><b style="font-size: 0.8em;color: black">I am lost and don’t know how to get back to where I need to be</b></p>
        <p>Virbela is a large place, however if you ever find you don’t know where you are. Use your GO TO menu to navigate back to campus. From campus you can then use the GO TO to get to any location in VirBELA.</p>
        
        <p><b style="font-size: 0.8em;color: black">VirBELA seems to be running very slow</b></p>
        <p>We recommend shutting down all other applications on your computer whilst running VirBELA to allow the application to run at full speed.</p>
    
    </div>
        
</div>