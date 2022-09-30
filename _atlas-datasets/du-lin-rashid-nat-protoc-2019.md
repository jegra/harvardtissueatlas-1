---
layout: secondary
title: Data
section_id: data
redirect_from:
  - /featured-paper/du-lin-rashid-2019/figures/
  - /featured-paper/du-and-lin-2019/figures/

data:
  publication:
    title: Qualifying antibodies for image-based immune profiling and multiplexed tissue imaging
    authors: Du Z, Lin JR, Rashid R, Maliga Z, Wang S, Aster J, Izar B, Sorger PK, Santagata S.
    journal: "Nat Protoc. 2019 Oct; 14(10): 2900-2930. PMID: 31534232."
    links:
      - Raw Data: https://www.synapse.org/#!Synapse:syn17865732/wiki/592782
      - Publication: https://www.nature.com/articles/s41596-019-0206-y

  stitched mosaic images:
    - title: TONSIL
      description: Representative t-CyCIF image acquired from a formalin-fixed, paraffin-embedded (FFPE) human tonsil tissue section stitched together using ASHLAR software from 224 fields acquired using a 40X/0.6NA objective.
      thumbnail file name: TONSIL_1.jpg
      links:
        - CyCIF tonsil image : osd-TONSIL_1
    - title: IHC Tonsil Sections
      description:
      thumbnail file name: TONSIL_IHC.jpg
      links:
        - IHC tonsil sections: osd-TONSIL_IHC
    - title: 'LUNG-3-PR: Primary lung squamous cell carcinoma  '
      description: Representative t-CyCIF image of a squamous cell carcinoma of the lung stitched together using ASHLAR software from 132 fields using a 40X/0.6NA objective.
      thumbnail file name: LUNG_3.jpg
      links:
        - CyCIF lung-3 image: osd-LUNG_3
    - title: 'LUNG-1-LN: Lung adenocarcinoma metastasis to lymph node'
      description: Representative t-CyCIF image of a lung adenocarcinoma metastasis to a lymph node stitched together using ASHLAR software from 80 fields using a 40X/0.6NA objective.
      thumbnail file name: LUNG_1.jpg
      links:
        - CyCIF lung-1 image: osd-LUNG_1
    - title: 'LUNG-2-BR: Lung squamous cell carcinoma metastasis to brain'
      description: Representative t-CyCIF image of a lung squamous cell carcinoma metastasis to the brain stitched together using ASHLAR software from 187 fields using a 40X/0.6NA objective.
      thumbnail file name: LUNG_2.jpg
      links:
        - CyCIF lung-2 image: osd-LUNG_2
---

{% include_relative TEMP-note-text.md %}

{% assign urlParts = page.url | split: '/' %}
{% assign sectionId = urlParts[-1] %}

{% include atlas-dataset-info.html
    sectionId=sectionId
    pubData=page.data
    thumbnailDir=sectionId %}

## Available images
{:.mt-5}

{% include atlas-dataset-cards.html
    sectionId=sectionId
    pubData=page.data
    thumbnailDir=sectionId %}
