## Contribute

### Add news

News are stored as `.yml` file under [_data/news.yml](_data/news.yml).

An entry looks like the following:

```yaml
- date: February 25, 2024
  title: "New website"
  content: The new website of our research group is launched!
```

### Add publications

Journal articles are stored as `.yml` file under [_data/publist.yml](_data/publist.yml).

An entry looks like the following:

```yaml
- title: "Evaluation of Methods and Metrics for Identifying Scattering Regime of Dielectric Particulate Medium"
  authors: Taufiq A, Erturk H, Yalcin RA
  image: icheatmasstransfer_154_2024.jpg
  link:
    url: https://doi.org/10.1016/j.icheatmasstransfer.2024.107386
    display: International Communications in Heat and Mass Transfer, Volume 154, 2024, 107386
  description: SSF estimates scattering coefficient and asymmetry parameter for dielectric particulate medium. Transport scattering coefficient is the proper metric for representing scattering regime. Solution of Maxwell’s equations is possible for finite sized particulate media. Coherent scattering leads to overestimation of scattering coefficient. Calculated asymmetry parameter depends on considered ensemble size.
  highlight: 1
```

If the journal article is not desired to be highlighted, then the following lines should be deleted: Image, description, highlight. All publication-related images (such as graphical abstracts) are stored under [images](images) folder. Furthermore, book chapters and patents can be added through lists under the markdown file [_pages/publications.md](_pages/publications.md).

### Add team members

Team members are stored as personalized markdown files under [_pages/team/_posts](_pages/team/_posts) folder.

An entry looks like the following:

```yaml
---
layout: member
category: staff
title: Hakan Ertürk
image: Hakan-Erturk.png
role: Professor
email: hakan.erturk@bogazici.edu.tr
permalink: 'team/hakan-erturk'
social:
    linkedin: https://www.linkedin.com/in/hakanerturk
    google-scholar: https://scholar.google.com/citations?user=0bWMg2kAAAAJ&hl=en&oi=ao
    researcherid: https://www.webofscience.com/wos/author/record/C-1238-2008
    orcid: https://orcid.org/0000-0001-5564-3845
    scopus: https://www.scopus.com/authid/detail.uri?authorId=35490437100
    research-gate: https://www.researchgate.net/profile/Hakan-Erturk
    github:
education:
- PhD in Mechanical Engineering, The University of Texas at Austin, Austin, TX, USA (2002)
- MS in Mechanical Engineering, Middle East Technical University, Ankara, Turkey (1997)
- BS in Mechanical Engineering, Middle East Technical University, Ankara, Turkey (1994)
interests:
- Design and control of thermal and energy systems
- Nanotechnology in energy applications
- Thermal management of opto/electronic systems
- Inverse problems of thermal design and sensing
---
```

Category should be labeled as "student" for all members, excluding the principal investigator. If an social media link is absent, then the relevant line can be deleted or the value after the key can be left empty, as provided in the example above for GitHub section. If the "interests" part is completely deleted, the program will understand this situation via a conditional statement, and research interests will not be visible to the end-user. All personal photos are stored under [images/team](images/team) folder.
