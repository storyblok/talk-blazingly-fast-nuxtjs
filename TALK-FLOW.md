# Live coding 
- create nuxt.js

`yarn create nuxt-app blazingly-fast-showcase`

## Jump to prepared repo with comments

- show the welcome screen

## Create Storyblok Space
- `Blazingly Fast - Showcase`
- preview sample content & components
- visual editor & content editor
- show preview TOKEN

## Setup the PREVIEW

`yarn add storyblok-nuxt`

- uncomment and add storyblok-nuxt plugin
- set the PREVIEW_TOKEN
  - change real path `/`
- show Nuxt.js Welcome Screen in Storyblok

## Create the default components & explain in Nuxt.js
- Page, Teaser, Grid, Feature
- nuxt.config.js -> plugins import compoennts.js

## Explain AsyncData
- Load from draft
- Save & Publish Event
- Input Event

## Create Article & FeaturedArticles in Storyblok
- Article
  - hero_image, title, intro, author, prose
- Create Article
- FeaturedArticles
  - articles - `articles/`
- Add FeaturedArticles to Page
  - explain those are references

## Create Article & FeaturedArticles in Nuxt.js
  - uncomment & explain resolve relations

## Show sorting

## Show v2 with localhost
local-ssl-proxy --source 3010 --target 3000 --cert localhost.pem --key localhost-key.pem
