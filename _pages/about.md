---
layout: about
title: Home
permalink: /
subtitle:
nav_order: 0

profile:
  align:
  image:
  name:
  image_circular: false # crops the image to make it circular

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: false # adds a vertical scroll bar if there are more than 3 news items
  limit: 3 # leave blank to include all the news in the `_news` folder
display_categories: [Lab Director, Administrator, PhD Students, Project Associates, M.Tech Students]
latest_posts:
  enabled: true
  scrollable: false # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

The **Spectrum Lab**
is a research group led by [Prof. Chandra Sekhar Seelamantula](https://ee.iisc.ac.in/chandra-sekhar-seelamantula/) in the [Department of Electrical Engineering](https://ee.iisc.ac.in/) at the [Indian Institute of Science](https://iisc.ac.in/). The lab focuses on problems in the intersection of computational imaging and machine learning.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path='assets/img/labphotos/icassp2025.jpg' title="ICASSP 2025" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Spectrum Lab, past and present, at <a href="https://2025.ieeeicassp.org/">ICASSP 2025</a>, in Hyderabad, India.
</div>

<div class="row align-items-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/labphotos/chitradurga-2024.JPG" title="Visiting the Challakere Campus" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Visiting IISc. Challakere Campus (May 2024)
        </div>
    </div>
    <div class="col-sm">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/labphotos/icassp-2019.JPG" title="ICASSP 2019" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            ICASSP 2019, Brighton, UK (May 2019)
        </div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/labphotos/iscs-2025.jpg" title="Spectrum Lab @ ISCS 2025" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Spectrum Lab @ ISCS 2025, Luxembourg (June 2025)
        </div>
    </div>
    </div>
</div>

# People
<hr style="border-top: 1px solid #bbb;">

<!-- pages/people.md -->
<div class="people">
  <!-- Display categorized people except Alumni -->
  {%- for category in page.display_categories %}
      <h2 class="category">{{ category }}</h2>
      {%- assign categorized_people = site.people | where: "category", category -%}
      {%- assign sorted_people = categorized_people | sort: "lastname" %}
      <!-- Generate cards for each person -->
      <div class="grid">
        {%- for person in sorted_people -%}
          {%- if person.show -%}
            {% include people.liquid %}
          {%- endif -%}
        {%- endfor %}
      </div>
  {% endfor %}
</div>
