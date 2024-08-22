---
layout: page
permalink: /repositories/
title: repositories
description: # Edit the `_data/repositories.yml` and change the `github_users` and `github_repos` lists to include your own GitHub profile and repositories.
nav: true
nav_order: 4
---

## GitHub Profile

You can find me on GitHub as [@WoutDLN](https://github.com/WoutDLN). I am also part of (and contributed to) the following GitHub Organizations:

- [SSLIS](https://github.com/SSLIS): aggregating repositories developed at the [Swedish School of Library and Information Science](https://www.hb.se/en/the-swedish-school-of-library-and-information-science-sslis/about-the-swedish-school-of-library-and-information-science/)
- [ESTS-Variants](https://github.com/ESTS-Variants): aggregating repositories developed for [Variants](https://journals.openedition.org/variants/1190), the Journal of the [European Society for Textual Scholarship](https://textualscholarship.eu/)
- [DH Benelux](https://github.com/DHBenelux): aggregating repositories developed for and by the [DH Benelux](https://dhbenelux.org/) community
- [Centre for Manuscript Genetics](https://github.com/centre-for-manuscript-genetics): aggregating repositories developed at the University of Antwerp's research centre fo the same name

## GitHub Repositories

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
