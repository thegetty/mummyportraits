This is the repository for “Mummy Portraits of Roman Egypt: Emerging Research from the APPEAR Project,” edited by Marie Svoboda and Caroline R. Cartwright. This digital book was first published August 25, 2020, by the J. Paul Getty Museum. It is available online at [http://www.getty.edu/publications/mummyportraits/](http://www.getty.edu/publications/mummyportraits/) and may be downloaded free of charge in multiple formats.

## About the Book

Once interred with mummified remains, nearly a thousand funerary portraits from Roman Egypt survive today in museums and galleries around the world, bringing viewers face-to-face with people who lived two thousand years ago. Until recently, few of these paintings had undergone in-depth study to determine how they were made.

An international collaboration known as APPEAR (Ancient Panel Paintings: Examination, Analysis, and Research) was launched in 2013 to promote the study of these objects and to gather scientific and historical findings into a shared database. The first phase of the project was marked with a two-day conference at the Getty Villa. Conservators, scientists, and curators presented new research on topics such as provenance and collecting, comparisons of works across institutions, and scientific studies of pigments, binders, and supports. The papers and poster presentations from the conference are collected in this publication, which offers the most up-to-date information available about these fascinating remnants of the ancient world.

## Using this Repository

This is one in series of multiformat publications using [Quire](http://www.getty.edu/publications/digital/platforms-tools.html), Getty’s new publishing framework. Quire is currently in private beta, with the goal of it being released as free and open source software in the future. In the meantime, users are encouraged to request access at http://bit.ly/quire-beta. This repository can also be run locally to build the online site (but not the PDF or ebook formats) with [Hugo](https://gohugo.io/), the [static site generator](https://www.smashingmagazine.com/2015/11/modern-static-website-generators-next-big-thing/) at the core of Quire.

We are dedicated to maintaining this publication for years to come at the permanent URL, [http://www.getty.edu/publications/mummyportraits/](http://www.getty.edu/publications/mummyportraits/), and in its various formats and incarnations. For any updates to the book, we will be following something between an app and traditional book publication model. Updates will only be made in regulated chunks as formal revisions and new editions and will always be thoroughly documented here in the repository, as well as in the revision history included with each of the book’s many formats.

The primary content pieces of the book can be found in the `data` and `content` directories. The master branch represents the current, published edition at all times, and the revisions branch, when present, will show changes currently under consideration. We invite you to submit suggestions or corrections via pull request on the revisions branch, by posting an issue, or by emailing us at [pubsinfo@getty.edu](mailto:pubsinfo@getty.edu).

## Development Notes

This project was last built with the following software versions:

- Quire 0.18.0
- Node 12.18.3 / npm 6.14.6
- Hugo 0.72
- PrinceXML 13.5
- Pandoc 2.10.1

While v0.18.0 of the core Quire Starter Theme was used, a number of customizations were made:

- Include custom, four-quadrant cover animation
- Remove page-level bibliography
- Add page-level copyright notice using a `copyright` attribute in the page yaml
- Link contributor names on individual pages to their biographies on the Contributors page
- Add custom pop-up definition and glossary shortcodes

Within the theme itself, changes were made to the `source/css/variables.scss` and `source/css/print.scss` files. Outside of the theme, customizations can be found in the project’s `layouts` directory, and in `static/css/custom.css`.

### Images Submodule

Many of figure images for *Mummy Portraits* are licensed from third parties for use exclusively in this publication. As such, they are kept in a separate, private repository, https://github.com/thegetty/mummyportraits-images/, which is linked to this main publication repository as a submodule in `static/img/figures/`. When cloning this repo for further development, you’ll permissions for the private repository and will need to clone recursively in order to clone both the main repo and the submodule.

```
git clone --recursive https://github.com/thegetty/mummyportraits.git
```

## License

© 2020 J. Paul Getty Trust

The text of this work and figs. 4.2–3, 4.10, 4.13, 8.3–4, 11.2–5, and 17.4a are licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). All other images are reproduced with the permission of the rights holders acknowledged in captions and are expressly excluded from the CC BY license covering the rest of this publication. These images may not be reproduced, copied, transmitted, or manipulated without consent from the owners, who reserve all rights.
