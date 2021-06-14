<p align="center">
  <a href="https://datamine.purdue.edu"><img width="100%" src="./banner.png" alt='Purdue University'></a>
</p>


---

**Website**: [https://the-examples-book.com](https://the-examples-book.com)

---

# docs-scraper

This is a fork of [the docs-scraper](https://github.com/meilisearch/docs-scraper) for [Meilisearch](https://www.meilisearch.com/). Meilisearch is a fantastic search solution that makes it very easy to integrate powerful and fast search capabilities into your website or project. docs-scraper is an associated project that makes it easy to scrape your website and update the search index. We've forked this repository to ensure that breaking changes aren't made suddenly and without warning.

## Run

To run this script, the following 2 environment variables are required to be set:

- `MEILISEARCH_API_KEY`
- `MEILISEARCH_HOST_URL`

`MEILISEARCH_API_KEY` is your Meilisearch instance's API key, and `MEILISEARCH_HOST_URL` is the URL where the Meilisearch instance is running. If running locally, the easiest way to set this up is to create a `.env` file with the required information. docs-scraper will automatically use the information therein.

```bash
MEILISEARCH_API_KEY=<api_key>
MEILISEARCH_HOST_URL=<host_url>
```

First, clone the repository.

```bash
git clone git@github.com:TheDataMine/docs-scraper.git
```

Then, to update the search index, run the following.

```bash
cd docs-scraper
pipenv install
pipenv run ./docs-scraper the-examples-book.config.json
```

Congratulations, the search index is now up-to-date.

<p align="center">&mdash; # &mdash;</p>
<p align="center"><i></i></p>