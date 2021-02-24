---
layout: ieeevr-default
---

<div>
    <h1 id="past-conferences"> what's happening now widget </h1>
    
    

    <p>Date/Time: <span id="datetime"></span></p>
    <script type="text/javascript">
        
        
        var today = new Date();
        var dt = today.toLocaleString(undefined, { timeZone: "Europe/Lisbon"});
        
        document.getElementById("datetime").innerHTML = dt.toLocaleString();

        
        
        document.write("<p><strong>");
        document.write(dt.toLocaleString());
        document.write("</strong></p>");

        
        var timeslot1 = Date.parse("2/24/2021, 5:00:00 AM");
        var timeslot2 = Date.parse("2/24/2021, 6:00:00 AM");
        
        console.log(timeslot1.toLocaleString());
        console.log(timeslot2.toLocaleString());
        console.log(dt.toLocaleString());
        console.log((dt > timeslot1) && (dt < timeslot2));
        
    </script>




</div>