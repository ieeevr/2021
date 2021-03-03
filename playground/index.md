---
layout: ieeevr-default
title: "Program Overview"
---

<h1>Data:</h1>

<script type="text/javascript">
    
    var txtFile = new XMLHttpRequest();
    txtFile.onload = function() {
        allText = txtFile.responseText;
        allTextLines = allText.split(/\r\n|\n/);

        for (var i = 0; i < allTextLines.length; i++) {
            document.body.innerHTML += allTextLines[i];
            document.body.innerHTML += '<br/>';
        }
    }

    txtFile.open("get", "http://ieeevr.org/2021/playground/data.csv", true);
    txtFile.send();

</script>



<p>End data</p>
