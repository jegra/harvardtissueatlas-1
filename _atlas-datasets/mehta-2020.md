---
layout: secondary
title: Data
section_id: data

data:
  publication:
    title: Targeting immunosuppressive macrophages overcomes PARP inhibitor resistance in _BRCA1_-associated triple-negative breast cancer
    description: Despite objective responses to PARP inhibition and improvements in progression-free survival compared to standard chemotherapy in patients with BRCA-associated triple-negative breast cancer (TNBC), benefits are transitory. Using high dimensional single-cell profiling of human TNBC, here we demonstrate that macrophages are the predominant infiltrating immune cell type in BRCA-associated TNBC. Through multi-omics profiling we show that PARP inhibitors enhance both anti- and pro-tumor features of macrophages through glucose and lipid metabolic reprogramming driven by the sterol regulatory element-binding protein 1 (SREBP-1) pathway. Combined PARP inhibitor therapy with CSF-1R blocking antibodies significantly enhanced innate and adaptive anti-tumor immunity and extends survival in BRCA-deficient tumors in vivo and is mediated by CD8+ T-cells. Collectively, our results uncover macrophage-mediated immune suppression as a liability of PARP inhibitor treatment and demonstrate combined PARP inhibition and macrophage targeting therapy induces a durable reprogramming of the tumor microenvironment, thus constituting a promising therapeutic strategy for TNBC.
    authors: Anita K. Mehta, Emily M. Cheney, Christina A. Hartl, Constantia Pantelidou, Madisson Oliwa,  Jessica A. Castrillon, Jia-Ren Lin, Katie E. Hurst, Mateus de Oliveira Taveira, Nathan T. Johnson, William M. Oldham, Marian Kalocsay, Matthew J. Berberich, Sarah A. Boswell, Aditi Kothari, Shawn Johnson, Deborah A. Dillon, Mikel Lipschitz, Scott Rodig, Sandro Santagata, Judy E. Garber, Nadine Tung, José Yélamos, Jessica E. Thaxton, Elizabeth A. Mittendorf, Peter K. Sorger, Geoffrey I. Shapiro and Jennifer L. Guerriero  
    journal: 'Nature Cancer. 2021; 2(1): 66-82. PMID: 33738458'
    links:
      - Publication: https://www.nature.com/articles/s43018-020-00148-7

  group object:
    Wildtype vs mutant:
      - title: _BRCA_-WT vs _BRCA1_-associated TNBC
        description:
        thumbnail file name: BRCA-WT-vs-BRCA1-associated-TNBC.jpg
        links:
          - CyCIF image: osd-BRCA-WT-vs-BRCA1-associated-TNBC

    _BRCA_-wildtype TNBC:
      - title: _BRCA_-WT TNBC 1
        description:
        thumbnail file name: BRCA-WT-1.jpg
        links:
          - CyCIF image: osd-BRCA-WT-1
      - title: _BRCA_-WT TNBC 2
        description:
        thumbnail file name: BRCA-WT-2.jpg
        links:
          - CyCIF image: osd-BRCA-WT-2
      - title: _BRCA_-WT TNBC 3
        description:
        thumbnail file name: BRCA-WT-3.jpg
        links:
          - CyCIF image: osd-BRCA-WT-3
      - title: _BRCA_-WT TNBC 4
        description:
        thumbnail file name: BRCA-WT-4.jpg
        links:
          - CyCIF image: osd-BRCA-WT-4
      - title: _BRCA_-WT TNBC 5
        description:
        thumbnail file name: BRCA-WT-5.jpg
        links:
          - CyCIF image: osd-BRCA-WT-5
      - title: _BRCA_-WT TNBC 6
        description:
        thumbnail file name: BRCA-WT-6.jpg
        links:
          - CyCIF image: osd-BRCA-WT-6

    _BRCA1_-associated TNBC:
      - title: _BRCA1_-associated TNBC 1
        description:
        thumbnail file name: BRCA1-associated-1.jpg
        links:
          - CyCIF image: osd-BRCA1-associated-1
      - title: _BRCA1_-associated TNBC 2
        description:
        thumbnail file name: BRCA1-associated-2.jpg
        links:
          - CyCIF image: osd-BRCA1-associated-2
      - title: _BRCA1_-associated TNBC 3
        description:
        thumbnail file name: BRCA1-associated-3.jpg
        links:
          - CyCIF image: osd-BRCA1-associated-3
      - title: _BRCA1_-associated TNBC 4
        description:
        thumbnail file name: BRCA1-associated-4.jpg
        links:
          - CyCIF image: osd-BRCA1-associated-4
      - title: _BRCA1_-associated TNBC 5
        description:
        thumbnail file name: BRCA1-associated-5.jpg
        links:
          - CyCIF image: osd-BRCA1-associated-5
      - title: _BRCA1_-associated TNBC 6
        description:
        thumbnail file name: BRCA1-associated-6.jpg
        links:
          - CyCIF image: osd-BRCA1-associated-6
      - title: _BRCA1_-associated TNBC 7
        description:
        thumbnail file name: BRCA1-associated-7.jpg
        links:
          - CyCIF image: osd-BRCA1-associated-7
      - title: _BRCA1_-associated TNBC 8
        description:
        thumbnail file name: BRCA1-associated-8.jpg
        links:
          - CyCIF image: osd-BRCA1-associated-8
      - title: _BRCA1_-associated TNBC 9
        description:
        thumbnail file name: BRCA1-associated-9.jpg
        links:
          - CyCIF image: osd-BRCA1-associated-9
      - title: _BRCA1_-associated TNBC 10
        description:
        thumbnail file name: BRCA1-associated-10.jpg
        links:
          - CyCIF image: osd-BRCA1-associated-10
---

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
