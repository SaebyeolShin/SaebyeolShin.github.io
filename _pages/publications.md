---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

\* indicates Equal Contribution

<table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">

  {% for post in site.publications reversed%}
  <tr>
    <td style="border: none; padding:2.5%;width:25%;vertical-align:middle;max-width:100px;max-height:100px">
      <img src="/{{post.image}}" alt="project image" style="width:auto; height:auto; max-width:100%;" />
    </td>
    <td style="border: none; padding:2.5%;width:75%;vertical-align:middle">
      <h3>{{post.title}}</h3>
      {{post.authors}}
      <br>
      <em>{{post.venue}}</em>, {{ post.date | date: "%Y" }}
      <br>
        {% if post.paper %}
          <a href="{{post.paper}}" style="background-color: white; color: #008CBA; border: 1px solid #008CBA; padding: 0px 10px; text-align: center; text-decoration: none; display: inline-block; margin-top:8px; border-radius: 5px;">paper</a>
        {% endif %}
        {% if post.code %}
          <a href="{{post.code}}" style="background-color: white; color: #008CBA; border: 1px solid #008CBA; padding: 1px 10px; text-align: center; text-decoration: none; display: inline-block; margin-left: 1px; margin-top:8px; border-radius: 5px;">code</a>
        {% endif %}
        {% if post.web %}
          <a href="{{post.web}}" style="background-color: white; color: #008CBA; border: 1px solid #008CBA; padding: 1px 10px; text-align: center; text-decoration: none; display: inline-block; margin-left: 1px; margin-top:8px; border-radius: 5px;">website</a>
        {% endif %}
        {% if post.video %}
          <a href="{{post.video}}">video</a>
        {% endif %}
        {% if post.poster %}
          / <a href="{{post.poster}}">poster</a>
        {% endif %}
        {% if post.slides %}
          / <a href="{{post.slides}}">slides</a>
        {% endif %}
        {% if post.dataset %}
          / <a href="{{post.dataset}}">dataset</a>
        {% endif %}
      <p></p>
      {{ post.excerpt }}
    </td>
  </tr>
  {% endfor %}
</table>
