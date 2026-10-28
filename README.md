# Rutgers AI Resources

A student-maintained guide to the generative AI tools, student offers, courses, and campus guidance available to Rutgers students. It is not affiliated with or endorsed by Rutgers University.

**Site:** <https://trian27.github.io/RutgersAIResources/>

## Contents

| Page | Source |
|:-----|:-------|
| Home | [`docs/index.md`](docs/index.md) |
| Rutgers tools: free assistants, campus software, Amarel, workshops | [`docs/rutgers-tools.md`](docs/rutgers-tools.md) |
| Student offers: free and discounted plans | [`docs/student-offers.md`](docs/student-offers.md) |
| Coding and data: coding assistants, free GPUs, cloud credits | [`docs/coding.md`](docs/coding.md) |
| Study and research | [`docs/study-research.md`](docs/study-research.md) |
| Learn AI: free courses | [`docs/learn-ai.md`](docs/learn-ai.md) |
| Using AI responsibly: integrity, data, citing AI | [`docs/responsible-use.md`](docs/responsible-use.md) |
| Tutorials: GitHub Copilot, Gemini Notebook | [`docs/tutorials/`](docs/tutorials/) |

## How it's built

GitHub Pages builds the site with Jekyll from `docs/` on `main`, using the [Just the Docs](https://just-the-docs.com/) remote theme (`docs/_config.yml`). The root `Gemfile` is only for local previews. [`.github/workflows/links.yml`](.github/workflows/links.yml) runs [lychee](https://github.com/lycheeverse/lychee) to check every link on pushes, pull requests, and once a month.

Preview locally with Ruby 3.2 or later and Bundler:

```sh
bundle config set --local path vendor/bundle
bundle install
bundle exec jekyll serve --source docs --destination _site
```

## Contributing

Suggestions and corrections are welcome. See [`docs/contributing.md`](docs/contributing.md) for what belongs on the site and how to submit changes. Every claim about price, eligibility, or data use should link to an official source.
