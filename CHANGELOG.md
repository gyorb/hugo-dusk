# Changelog

## [Unreleased]

### Changed
  * main content is under blog instead of post
  * replaced exampleSite

### Added
  * add separate optional main page instead of the list of posts set it with: "enable_separate_main_page"
  * add separate blog layout
  * add last modification date to the post footer
  * add support to syndicate links
  * extend default archetype template
  * separate description value for each post (metadata)
  * support callout blockquotes 
  * support and separate page for micro posts
  * related content is visible at the bottom of a post

## [1.4.0] - 2024-10-21

### Added
  * [Mastodon](https://joinmastodon.org/) [verification](https://joinmastodon.org/verification)
  * [Fediverse creator tag](https://blog.joinmastodon.org/2024/07/highlighting-journalism-on-mastodon/)

### Changed
  * Simplify design
    * Remove social links from the top and reading time
    * change date format

## [1.3.0] - 2024-09-13

### Changed
  * fine-tune cold dark theme
  * update readme

## [1.2.0] - 2024-09-12

### Added
  * Show categories and series for the posts
  * [Utterances](https://utteranc.es/) comments support by @Jarijaas
  * design update:
    - improved instagram card style
    - readability and contrast updates
    - titles, tags, list of posts are not so dense as before
    - default colors were fine tuned
    - some small layout changes
    - smaller theme updates
  * new dark theme: cold-dark.css

### Changed
  * Configuration example for syntax highlight
  * Theme colors can be changed in a custom css file
  * minimal required Hugo version is v0.57.2
  * sort posts/pages on the error page by last modification date
  * update exampelSite config
  * use shorthand padding syntax

### Fixed
  * fix: update to hugo 1.33.0
  * fix date format for the post footer
  * fix breaking change in mainSections introduced in Hugo v0.57.0
  * deprecation warnings during site build with v0.55 and newer
  * optimize image size when viewed on mobile devices


## [1.1] - 2017-11-22
### Added
  * Theme colors can be changed in the config file
  * Makefile for easier development

### Changed
  * highlightjs was removed, builtin Chroma is used for syntax highlight
  * Position of the read more links is closer to the text
  * Abbreviations are used for social media names under the site title
  * Disqus localhost check was removed
  * Default archetype was extended and the new format is yaml

### Fixed
  * missing closing html tag


## [1.0.1] - 2017-08-24
### Fixed
  * Tag URLs by @Butt4cak3
  * gitlab social links by @CrazedProgrammer
  * gitlab url by @CrazedProgrammer


## [1.0] - 2017-04-22
### Added
  * Responsive minimalistic design
  * Syntax highlight with [highlight.js](https://highlightjs.org/)
  * [OpenGraph](http://ogp.me/) support
  * [Twitter cards](https://dev.twitter.com/cards/overview) support
  * [Disqus](https://disqus.com/) comments
  * [Google analytics](https://www.google.com/analytics/) (async)
  * Configrable pagination for posts
  * Lazy menu
  * Custom 404 page
