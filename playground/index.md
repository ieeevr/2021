---
layout: ieeevr-default
---

<div>
    <h1 id="past-conferences"> what's happening now widget </h1>
    
    

    <p>Date/Time: <span id="datetime"></span></p>
    <script type="text/javascript" src="https://unpkg.com/moment">
        
        
        var today = new Date();
        var dt = today.toLocaleString(undefined, { timeZone: "Europe/Lisbon"});
        
        document.getElementById("datetime").innerHTML = dt.toLocaleString();

        
        
        document.write("<p><strong>");
        document.write(dt.toLocaleString());
        document.write("</strong></p>");

        
        var timeslot1 = Date.parse('24 Feb 2021 01:00:00 Europe/Lisbon');
        var timeslot2 = Date.parse('24 Feb 2021 02:00:00 Europe/Lisbon');
        var DateNow = Date.parse('24 Feb 2021 01:30:00 Europe/Lisbon');
        
        document.write("<p>");
        document.write(DateNow);
        document.write("</p>");
        
        document.write("<p>");
        document.write((timeslot1 > DateNow) && (DateNow < timeslot2));
        document.write("</p>");
        
    </script>




</div>