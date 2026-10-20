# mstate2: a demonstration

Slides introducing second-order Markov multistate models and the R package
[**mstate2**](https://github.com/jcarmezim/mstate2), illustrated with the DIVINE
cohort of patients hospitalised with COVID-19.

**Online presentation:** https://USER.github.io/REPOSITORY/

## Contents

| File | Content |
|---|---|
| `mstate2_presentation.qmd` | Quarto source of the slides (revealjs) |
| `mstate2-theme.scss` | theme |
| `WWW/` | title-slide template and institutional logos |
| `index.html` | rendered, self-contained presentation |

## Rendering

The slides use the version of `mstate2` on the `master` branch and the DIVINE
multistate extract (`MSM_Data.RData`), which is distributed by the DIVINE
project and is **not** included in this repository.

```r
remotes::install_github("jcarmezim/mstate2")
```

```sh
# with MSM_Data.RData in this folder, or its path in MSTATE2_DIVINE_DATA
quarto render mstate2_presentation.qmd
```

The output is `index.html`, a single file with every image and style embedded.

## Publishing with GitHub Pages

Settings → Pages → *Deploy from a branch* → branch `main`, folder `/ (root)`.
