---
layout: secondary
title: Data

data:
  publication:
    title: Spatial intra-tumor heterogeneity is associated with survival of lung adenocarcinoma patients
    authors: 'Hua-Jun Wu, Daniel Temko, Zoltan Maliga, Andre Moreira, Emi Sei, Darlan Conterno Minussi, Jamie Dean, Charlotte Lee, Qiong Xu, Guillaume Hochart,Connor Jacobson, Clarence Yapp, Denis Schapiro, Peter Sorger, Erin H. Seeley, Nicholas Navin, Robert J. Downey, and Franziska Michor'
    journal: 'Forthcoming in Cell Genomics'
    description: Intratumor   heterogeneity   (ITH)   of   human   tumors   is   important   for   tumor progression,   treatment   response,   and   drug   resistance.   However,   the   spatial distribution of ITH remains incompletely understood. Here, we present spatial analysis of ITH in lung adenocarcinomas from 147 patients using multi-region mass spectrometry of >5000 regions, single cell copy number sequencing of ~2000 single cells, and cyclic immunofluorescence of >10 million cells. We identified two distinct spatial   patterns   among   tumors,   termed   clustered   and   random   geographic diversification (GD). These patterns were observed in the same samples using both proteomic and genomic data. The random proteomic GD pattern, which is characterized by decreased cell adhesion and lower levels of tumor-interacting endothelial cells, was significantly associated with increased risk of recurrence or death in two independent patient cohorts. Our study presents comprehensive spatial mapping of ITH in lung adenocarcinoma and provides insights into the mechanisms and clinical consequences of geographic diversification of intratumor heterogeneity.
---
{% assign urlParts = page.url | split: '/' %}
{% assign sectionId = urlParts[-1] %}

{% include atlas-dataset-info.html
    sectionId=sectionId
    pubData=page.data
    thumbnailDir=sectionId %}

### Contents
* [Data Explorations](#data-explorations)
* [Data Overviews](#data-overviews)
* [Data Access](#data-access)

## Data Explorations
**Data Explorations are like museum guides and exploit the digital docents in MINERVA to guide readers through the complexities of a large image dataset via a series of narrated stories and waypoints.**

{%
    assign stories = site.data-cards
    | where_exp: "item", "item.url contains 'wu-temko-maliga-2022/'"
    | where_exp: "item", "item.hide != true"
%}

<section class="data-cards">
    <div class="data-cards__inner">
        <div class="data-cards__items">
            {% for s in stories %}
            {% unless s.url contains '-overview' %}
            {% include data-card.html content=s %}
            {% endunless %}
            {% endfor %}
        </div>
    </div>
</section>

## Data overviews

**Data Overviews provide access to minimally processed Level 2 images with no annotation or quality control. Click any of the following thumbnail images for an interactive view of the full-resolution images.**

{%
    assign overviews = site.data-cards
    | where_exp: "item", "item.url contains 'wu-temko-maliga-2022/'"
    | where_exp: "item", "item.hide != true"
    | where_exp: "item", "item.url contains '-overview'"
%}

<section class="data-cards">
    <div class="data-cards__inner">
        <div class="data-cards__items">
            {% for o in overviews %}
            {% include data-card.html content=o %}
            {% endfor %}
        </div>
    </div>
</section>

### Data Access
<details>
    <summary>Download the primary data</summary>
<div markdown="1">
{% include_relative wu-temko-maliga-2022-file-list.md %}
</div>
</details>