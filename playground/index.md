---
layout: ieeevr-default
---

<div>
    <h1 id="past-conferences"> what's happening now widget!!! </h1>
    
    

    <script>
        document.write("<p>");
    
        var d = new Date();
        var s = d.toLocaleDateString(undefined, { timeZone: "Europe/Lisbon"});
    
        var displayTime = s.getDate() + "/"
                + (s.getMonth()+1)  + "/" 
                + s.getFullYear() + " @ "  
                + s.getHours() + ":"  
                + s.getMinutes() + ":" 
                + s.getSeconds();
        
        document.write(displayTime);
        
        document.write("</p>")
    
    </script>




</div>