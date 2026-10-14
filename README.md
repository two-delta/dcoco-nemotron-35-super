# DCOCO × NVIDIA Nemotron 3.5 Super

Blog post on making NVIDIA Nemotron 3.5 Super faster with DCOCO, published at
**https://two-delta.github.io/dcoco-nemotron-35-super/**. The method is described in
[DCOCO: Contextual Correction of Parallel Drafts for Speculative Decoding](https://arxiv.org/abs/2610.12570)
and its main project page is [two-delta/dcoco-blog](https://github.com/two-delta/dcoco-blog).

`site/` is the whole site: one self-contained `index.html` plus its figures and logos. Every push to
`main` deploys it through `.github/workflows/pages.yml`. The repository is public, and so is the site.

## Preview

```bash
python3 -m http.server 8000 --directory site
```

## Figures and logos

Formulas are typeset with KaTeX (loaded from jsDelivr). Figure 1 ("These key is missing" → "These keys are missing") is an inline SVG animation in
`index.html`. Tables 1 and 2 are HTML. Everything else is a PNG:

| File | Content |
| --- | --- |
| `site/figures/main_figure.png` | Figure 2: DCOCO architecture and prefix-first selection |
| `site/figures/figure3_single_request.png` | Figure 3: mean throughput at C = 1, T = 0 and T = 1 (also the og:image) |
| `site/figures/figure4_concurrency.png` | Figure 4: throughput vs. concurrency |
| `site/figures/figure5_acceptance.png` | Figure 5: acceptance length vs. concurrency |
| `site/logos/td.png` | Two Delta logo, left of the NVIDIA logo (transparent, downscaled to 224px) |
| `site/logos/nvidia.png` | NVIDIA logo above the title, cropped from NVIDIA's vertical screen logo |

Styling is the same as the DCOCO project page (Roboto / Roboto Mono, same layout and type scale); only the
palette is green instead of blue.
