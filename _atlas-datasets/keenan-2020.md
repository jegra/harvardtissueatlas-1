---
layout: secondary
title: Data
section_id: data

data:
  publication:
    title: Clinical efficacy and molecular response correlates of the Wee1 inhibitor adavosertib with cisplatin in metastatic triple-negative breast cancer (mTNBC)
    authors: Keenan T., Li T., Vallius T., Guerriero J.L., Tayob N., Kochupurakkal B., Davis J., Pastorello R., Tahara R.K., Anderson L., Conway J., He M.X., Shannon E., Godin R.E., Sorger P.K., D’Andrea A., Overmoyer B.,  Winer E.P., Mittendorf E.A., Van Allen E., Shapiro G.I., Tolaney S.M.
    journal: "Clinical Cancer Research, 2(1), 66-82. PMID: 33257427"
    description: Selective inhibition of the negative cell cycle regulator WEE1 may enhance the efficacy of DNA-damaging agents by reducing DNA damage repair. These are multiplexed cyclic immunofluorescence on paired pre- and post-WEE1 inhibitor tumor biopsies, from the first phase II study assessing the efficacy of the WEE1 inhibitor adavosertib with cisplatin in metastatic triple-negative breast cancer (mTNBC). Among patients with mTNBC treated with 0-1 prior lines, adavosertib combined with cisplatin narrowly missed the prespecified ORR cutoff of > 30%. The finding of immune infiltrated tumors in patients with clinical benefit to therapy requires validation in future studies.
    links:
      - Publication: https://doi.org/10.1158/1078-0432.CCR-20-3089

  stitched mosaic images:
    - title: Clinical Benefit - Cisplatin Biopsy
      description: CyCIF image of a biopsy from a patient with triple-negative breast cancer (TNBC) liver metastasis. This biopsy was obtained after the first infusion of Cisplatin (Cis) chemotherapy, before Wee1 inhibitor therapy.
      thumbnail file name: cis.jpg
      links:
        - CyCIF image: osd-cis
    - title: Clinical Benefit - Cis Wee1i Biopsy
      description: CyCIF image of a biopsy from a patient with triple-negative breast cancer (TNBC) liver metastasis, after combination therapy with Cisplatin and the Wee1 inhibitor Adavosertib.
      thumbnail file name: Wee1.jpg
      links:
        - CyCIF image: osd-Wee1
    - title: No Clinical Benefit - Cisplatin Biopsy
      description: CyCIF image of a biopsy from a patient with triple-negative breast cancer (TNBC) liver metastasis. This biopsy was obtained after the first infusion of Cisplatin (Cis) chemotherapy, before Wee1 inhibitor therapy.
      thumbnail file name: 25_C1_a.jpg
      links:
        - CyCIF image: osd-25_C1_a
    - title: No Clinical Benefit - Cis Wee1i Biopsy
      description: CyCIF image of a biopsy from a patient with triple-negative breast cancer (TNBC) liver metastasis, after combination therapy with Cisplatin and the Wee1 inhibitor Adavosertib.
      thumbnail file name: 25_C2_b.jpg
      links:
        - CyCIF image: osd-25_C2_b
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
