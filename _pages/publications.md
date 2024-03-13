---
title: "Publications"
layout: gridlay
excerpt: "TESLab - Publications"
sitemap: false
permalink: /publications/
---

# Publications

The full list of journal articles is given below this page, these are also accessible on Prof. Hakan Erturk's <a href="https://scholar.google.com/citations?user=0bWMg2kAAAAJ&hl=en">Google Scholar</a> profile.

## Group highlights

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <b> <pubtit>{{ publi.title }}</pubtit> </b>
  <img src="{{ site.url }}{{ site.baseurl }}/images/{{ publi.image }}" class="img-responsive" width="100%" margin="30px" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

## Book Chapters/Sections

1.	Ertürk H, Howell JR, 2018, “Monte Carlo methods for Radiative Transfer”, Springer-Meteor’s Handbook of Thermal Sciences and Engineering, ed. F. Kulacki, pp.1201-1242.
2.	Hottel HC, Sarofim AF, Noble JJ, and Ertürk H, 2018, “Radiant Heat Transfer”, Section 2.3 in Marks’ Standard Handbook for Mechanical Engineers – Edition 12, eds.  AM Sadegh,  WM Worek, McGraw-Hill Book Co., pp.160-176.   
3.	Loke V, Erturk H, Menguc MP, 2023, Discrete Dipole Approximation with Surface Interactions, Light Plasmonics and Particles, eds. MP. Menguc, M. Francourt, Elsevier, pp.199-221.  

## Patents

1.	Yalcin, RA, Erturk, H, 2021, “Çok Katlı Seralar için bir Işıklandırma Sistemi”, TR-patent no. 2019 04787.
2.	Yalcin, RA, Erturk, H, 2020, “Lighting system for multi-layer greenhouses”, International Patent no. WO2020204858-A1.  
3.	Li, Z., Hsieh, C-C., Hu, J., Ertürk, H. and Chen, G., 2013, “Method for cooling ultramobile device used in web browsing, involves attaching microfins to distribution layer and applying force to microfins”, US Patent No. US8482922-B2.
4.	Li, Z., Hsieh, C-C., Hu, J., Ertürk, H. and Chen, G., 2011, “Ultramobile device passive cooling apparatus, has plane microfins attached to external wall of enclosure of ultramobile device, where in-plane thermal conductivity of microfins is higher than out-of-plane thermal conductivity of microfins”, US Patent No. US8054629-B2.
5.	Sauciuc, I., Chrysler, G.M., Ertürk, H., 2009, “Piezoelectricity air jet enhancement mode cooling apparatus for electronic device has multiple-layered leads which are laminated and developed in central opening surrounding piezoelectric layer”, US Patent No. US7633753-B2; Korean Patent no KR1031487-B1; Chinese Patent nos. CN101516173-A, CN101516173-B.
6.	Ertürk, H., Sauciuc, I., 2008, “Piezoelectric fan has piezoelectric sensor patch that is arranged adjacent to piezoelectric actuator patch and blade”, Korean Patent No. KR1004161-B1; Chinese Patent No. CN101354045-A.
7.	Ertürk, H., Chrysler, G.M., Sauciuc, I., 2008, “Method and System to Cool Memory”, US Patent No. US7457116-B2.
8.	Ertürk, H., Sauciuc, I., 2008, “Heat Dissipating Device with Enhanced Boiling/Condensation Structure”, US Patent No. 7353860-B2; Taiwanese Patent No. 293018-B1; International Patent No. WO2006007163-A1; Korean Patent No. KR2007017205-A; Chinese Patent nos. CN1969382-A, CN1969382-B; German Patent nos. DE112005001365-T5, DE112005001365-B4.
9.	Ertürk, H., Sauciuc, I., 2008, “Heat Dissipating Device with Enhanced Boiling/Condensation Structure”, US Patent No. 7327572-B2.  
10.	Ertürk, H., Sauciuc I., 2007, “Cooling Integrated Circuits Using a Cold Plate with Two Phase Thin Film Evaporation”, US Patent No. 7265979-B2.
11.	Ertürk H., Sauciuc I., Unrein, E. J., 2005, “An Apparatus and Method for Cooling Integrated Circuit Devices”, US Patent No. 6917522-B1.

## Journal Articles

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
