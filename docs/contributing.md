---
title: Contributing
nav_order: 9
description: "How to suggest a resource, report a broken link, or edit this site."
last_modified_date: 2026-10-28
---

# Contributing
{: .no_toc }

This site stays useful only if it stays current. Corrections and suggestions are welcome from anyone.
{: .fs-6 .fw-300 }

1. TOC
{:toc}

---

## Suggest a resource or report a problem

[Open an issue](https://github.com/Trian27/RutgersAIResources/issues/new/choose) and include a link to the official page that supports the change. This works for new resources, broken links, expired offers, and outdated instructions.

## Edit a page

Each page has an **Edit this page on GitHub** link at the bottom. To make a change:

1. Fork the [repository](https://github.com/Trian27/RutgersAIResources) and edit the Markdown file under `docs/`.
2. Update `last_modified_date` in the page's front matter to the date you checked the facts.
3. Open a pull request that says what changed and links to the sources.

## What belongs here

A resource should be:

- **Useful to Rutgers students:** free, free with a Rutgers account, or discounted for students. Paid tools belong only when they are the clear standard for a task.
- **Verifiable:** every claim about price, eligibility, deadlines, or data use links to the vendor's or university's own page, not a blog post or reseller.
- **Current:** the offer is open now. Note the end date if there is one, and remove an offer once it ends.

Entries are short: what the tool does, who qualifies, how to get it, and any data or course-policy caveat. Avoid exact usage limits and model names unless they matter, because they change every few months.

## Preview the site locally

The site uses [Jekyll](https://jekyllrb.com/) with the [Just the Docs](https://just-the-docs.com/) theme, and GitHub Pages builds it from the `docs/` folder on `main`. To preview your changes, install Ruby 3.2 or later and Bundler, then run from the repository root:

```sh
bundle config set --local path vendor/bundle
bundle install
bundle exec jekyll serve --source docs --destination _site
```

Then open <http://localhost:4000/RutgersAIResources/>.

A GitHub Actions workflow checks every link on pull requests and once a month.
