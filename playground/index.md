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

        
        
        
        
        document.write("<p>");
        document.write(moment().format('MMMM Do YYYY, h:mm:ss a'));
        document.write("</p>");
        
    </script>




</div>