---
layout: ieeevr-default
title: "IEEEVR 2021"
---

<!--
<div class="notice--warning">
    <strong style="color: red">Important notice:</strong>
    <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer suscipit pharetra lectus ut scelerisque. Suspendisse fermentum fringilla tellus, ac malesuada lectus aliquet tincidunt. Donec aliquam mollis efficitur. Etiam non sapien nisi.
    </p>
</div>
-->

<style>
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

    /* show more show less */
    @mixin truncate($rows, $line-height, $background: '') {
  position: relative;
  overflow: hidden;
  max-height: $line-height * $rows;
  line-height: $line-height;

  &:after {
    content: "";
    position: absolute;
    right: 0;
    bottom: 0;
    width: 100px;
    height: $line-height;

    @if $background != '' {
      background: linear-gradient(to right, rgba($background, 0) 0%, rgba($background, 1) 100%);
    }
  }

  @supports (-webkit-line-clamp: $rows) {
    display: -webkit-box;
    -webkit-line-clamp: $rows;
    -webkit-box-orient: vertical;

    &:after {
      display: none;
    }
  }
}

.show-hide-text {
  display: flex;
  flex-wrap: wrap;

  a {
    order: 2;
  }

  p {
    @include truncate(3, 20px, #fff); // rows, line-height, gradient fallback
  }
}

.show-less {
  display: none;

  &:target {
    display: block;

    ~ p {
      display: block;
      max-height: 100%;
    }

    + a {
      display: none;
    }
  }
}

    
</style>



<div class="show-hide-text wrapper">
  <a  id="show-more" class="show-less" href="#show-less">Show less</a>
  <a  id="show-less" class="show-more" href="#show-more">Show more</a>
  <p>
    Lorem Ipsum is simply dummy text of  the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
  </p>
</div>


<div>

    <div class="notice--info">
        <strong>Registration Information (15 Mar 2021):</strong>
        <p>
            The <strong>Advance Registration</strong> deadline was postponed to <strong>March 25th</strong>!!
            Register <a href="/2021/attend/registration/">here</a>.
        </p>
    </div>

    <div class="notice--info">
        <strong>Registration Information (24 Feb 2021):</strong>
        <p>
            Registration is now open!! You can consult the fee schedule and registration form <a href="/2021/attend/registration/">here</a>.
        </p>
    </div>

    <span id="more">

        <div class="notice--info">
            <strong>Registration Information (20 Feb 2021):</strong>
            <p>
                Due to the severe weather conditions in the USA, posting the registration form is delayed, since the support team is operating out of Dallas, TX. We expect the form to be up early next week. Thank you very much for your patience and understanding.
                You can consult the conference's fee schedule <a href="/2021/attend/registration/">here</a>.
            </p>
        </div>

        <div class="notice--info">
            <strong>Important Information:</strong>
            <p>
                Given the evolution of the pandemic, and following recommendations from public health authorities, VR 2021 will be all virtual, from March 27-April 3. We will process submissions as planned for different tracks. Stay tuned for more information!
            </p>
        </div>
    </span>


</div>


<br />
<div>
    <h1>Come and Join Us</h1>

    <!--    
    <p>
        Present your latest and greatest work at IEEE VR 2021. We are planning for VR 2021 to occur in both physical and virtual spaces.  The physical conference will be held at the <a href="https://tecnico.ulisboa.pt/en/">Instituto Superior Técnico</a>, one mile from the Lisbon airport, superbly located in downtown Lisbon. The sunniest European capital, Lisbon is one of the world’s most ancient cities, with a very rich history. Our goal is for IEEE VR 2021 to combine the best of traditional face-to-face meetings, while following the historical footsteps of the Virtual Experience of VR 2020 in Atlanta. The conference will take place from 27 of March to April 3rd, during Easter break.  Come join us for an unforgettable experience and explore the virtuality continuum in the premier event covering extended reality, featuring oral presentations, posters, research demos, tutorials, and workshops. 
    </p>
-->
    <p>
        Present your latest and greatest work at IEEE VR 2021. The conference will be virtual. Our goal is for IEEE VR 2021 to provide the best virtual experience, while following the historical footsteps of the Virtual Experience of VR 2020 in Atlanta. The conference will take place from 27 of March to April 3rd, during Easter break. Come join us for an unforgettable experience and explore the virtuality continuum in the premier event covering extended reality, featuring oral presentations, posters, research demos, tutorials, and workshops.
    </p>

</div>

<div>
    <h2>
        <a href="https://www.virbela.com/" target="_blank">
            <img style="width: 20%;" src="/2021/assets/images/sponsors/Virbela-logo.png" alt="Virbela Logo">
        </a>
    </h2>
    <div class="video-container">
        <iframe src="https://www.youtube.com/embed/TuOBgzJeQj0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

    </div>


    <p>
        Virbela builds engaging virtual worlds for remote work, learning, and events. Founded in 2012 by a team of behavioral psychologists, Virbela’s mission is to help organizations and people thrive in a remote-first future. Virbela is excited to partner with the iLRN team to provide the IEEE Conference with a platform to foster collaboration and networking.
    </p>
    <p>
        To learn more, visit virbela.com and follow us on <a href="https://twitter.com/VirbelaHQ" target="_blank">Twitter</a> and <a href="https://www.linkedin.com/company/virbela/" target="_blank">LinkedIn</a>.
    </p>
    <div style="">
        <center>
            <p style="font-size: 20px;">
                <a href="/2021/attend/virbela-instructions/" class="btn btn--primary" style="">Getting Started with Virbela</a>
            </p>
        </center>
    </div>
</div>
