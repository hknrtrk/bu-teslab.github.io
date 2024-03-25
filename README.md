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
