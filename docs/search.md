---
title: Documentation Search
permalink: /documentation-search.html
---
# Documentation Search

Doctory Jekyll has built-in documentation search powered by [Algolia](https://www.algolia.com/). All your docs are automagically reindexed on every push. Here's what you need to do to enable this.

## Set up Algolia

Head to Algolia's [website](https://www.algolia.com/) and login/signup. Go to [API keys section](https://www.algolia.com/api-keys) of the dashboard. You will need your Algolia **Application ID** and **Search only API key**. Then head to **_config.yaml** and update things accordingly:

```yaml
algolia:
  application_id:    APPLICATION_KEY
  index_name:        INDEX_NAME
  read_only_api_key: READONLY_API_KEY
  excluded_files:
    - 404.html

```

## Travis + Algolia

In the previous section, we have set up search related parts of the equation. Now we need to figure out how to ask Algolia to index your documentation. Automagically!

You will need to setup CI for your repo using [Travis CI](https://travis-ci.org/). CI configuration is already included inside ```.travis.yml``` file. You will need to add your repository on the site and add add an environmental variable on the project settings page. The var must be called ```ALGOLIA_API_KEY``` and should point to an Aloglia Key with write permissions. You can set it up in _Restricted Keys_ section of [API keys](https://www.algolia.com/api-keys). Refer to [Algolia Search for Jekyll](https://github.com/algolia/algoliasearch-jekyll) project for more information.

## Profit

With both configurations in place, your docs are re-indexed on every git push and are searchable through the search box in the sidebar.