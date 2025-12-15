---
title: Services
layout: services
description: Services
intro_image: "images/illustrations/developer.svg"
intro_image_absolute: false
intro_image_hide_on_mobile: true
---


<div class="intro">
  <div class="container">
    <div class="row justify-content-start">

      <div class="col-12 col-md-7 col-lg-6 order-2 order-md-1">
        <h1>Services that grow with you</h1>

        <p>
          GreenSeal.dev provides <strong>practical, measured, and engineering-driven services</strong>
          to reduce energy consumption and infrastructure costs across AI and cloud systems.
        </p>

        <p>
          Our services deliver value quickly — from fast diagnostics to hands-on optimization
          and long-term efficiency strategies.
        </p>

        {% include book-a-call.html %}

    </div>
{% if page.intro_image %}
  <div class="col-12 col-md-5 col-lg-6 order-1 order-md-2 position-relative">
    <img 
      alt="{{ page.title }}" 
      class="intro-image
        {% if page.intro_image_absolute %} intro-image-absolute{% endif %}
        {% if page.intro_image_hide_on_mobile %} intro-image-hide-mobile{% endif %}"
      src="{{ page.intro_image | relative_url }}" 
    />
  </div>
{% endif %}
    </div>
  </div>
</div>
<div class="strip strip-grey">
  <div class="container pt-6 pb-6 pb-md-10">
    <div class="row justify-content-start">
<!-- <div class="container pt-6 pb-6"> -->
  <!-- <div class="row strip-grey"> -->
    <h2>Core Services</h2>
     {% assign sorted_services = site.services | sort: "weight" %}
     {% for service in sorted_services %}
    <div class="col-12 col-md-6 mb-3">
      <div class="service service-summary">
        <div class="service-content">
          <h2 class="service-title">
            <a href="{{ service.url | relative_url }}">{{ service.title }}</a>
          </h2>
          <p>{{ service.summary | default: service.excerpt | markdownify | truncatewords: 70 }}</p>
          <p>
          <a href="{{ service.url | relative_url }}">👉 Learn more about this service.</a>
          </p>
        </div>
      </div>
    </div>
    {% endfor %}
        {% include book-a-call.html %}
  </div>
</div>
</div>
<div class="strip ">
  <div class="container pt-6 pb-6 pb-md-10">
    <div class="row justify-content-start">

        <h2>Education & Awareness</h2>

        <h3>🎤 Talks & Keynotes</h3>
        <p>
          High-level sessions on sustainable software and AI efficiency for technical
          and non-technical audiences.
        </p>

        <h3>🧑‍🏫 Training & Workshops</h3>
        <p>
          Hands-on workshops for developers, engineers, and managers focused on
          energy-efficient systems.
        </p>

        <h3>📅 Not sure where to start?</h3>
        <p>
          The <strong>Free Efficiency Assessment</strong> is the fastest way to understand
          your optimization potential.
        </p>

        {% include book-a-call.html %}

    </div>
</div>
</div>

                                
