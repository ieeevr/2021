---
layout: ieeevr-default
title: "Twitch Playground"
---

<div>
    
    <div>
        <h1>Session A</h1>
        <div id="session_A"></div> 
        <h2>Details</h2>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec venenatis diam eu ultrices accumsan. Suspendisse fermentum urna ac pulvinar lobortis. Duis finibus tellus id placerat consectetur. Donec at efficitur arcu.
        </p>
    </div>
    <div>
        <h1>Session B</h1>
        <div id="session_B"></div> 
        <h2>Details</h2>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec venenatis diam eu ultrices accumsan. Suspendisse fermentum urna ac pulvinar lobortis. Duis finibus tellus id placerat consectetur. Donec at efficitur arcu.
        </p>
    </div>
    <div>
        <h1>Session C</h1>
        <div id="session_C"></div>   
        <h2>Details</h2>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec venenatis diam eu ultrices accumsan. Suspendisse fermentum urna ac pulvinar lobortis. Duis finibus tellus id placerat consectetur. Donec at efficitur arcu.
        </p>
    </div>

    <script src="https://embed.twitch.tv/embed/v1.js"></script>

    <script type="text/javascript">
      new Twitch.Embed("session_A", {
        width: "100%",
        height: 480,
        channel: "ieeevr_test",
        muted: true,
      });
      new Twitch.Embed("session_B", {
        width: "100%",
        height: 480,
        channel: "ieeevr_test",
        muted: true,
      });
      new Twitch.Embed("session_C", {
        width: "100%",
        height: 480,
        channel: "ieeevr_test",
        muted: true,
      });
    </script>

</div>