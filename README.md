# Dude.fi
## Website redesign

This is a working copy of the website for [Digitoimisto Dude Oy](https://github.com/digitoimistodude) *(simply "Dude" - a Finnish digital agency)*.

## Table of contents

1. [Background story](#background-story)
  1. [Before GitHub](#before-github)
  2. [What's ignored](#whats-ignored)
2. [Features overview](#features-overview)
4. [Tools used](#tools-used)
5. [Building blocks](#building-blocks)
6. [Server stack](#server-stack)
7. [Building instructions](#building-instructions)

![Screenshot](https://dl.dropboxusercontent.com/u/18447700/dude.fi-2017.png "Screenshot")

## Background story

Dude built their first website when the company was formed in 2013. It was quite simple, but we needed it fast. Next, careful design we released after one year. And it was awesome. However, when things changed and there were suddendly 4 dudes instead of 2 in late 2015, we started to plan redesigning our website in early 2016.

We made quite a lot of planning in the spring and during the summer we started to work on the redesign. Summer died fast, so obviously got a bit stuck in the fall. When christmas holidays finally came, we continued with the site. Full blast in January, and boom! - the site was finally ready for the public to see.

### Before GitHub

Before releasing the dude.fi code in GitHub, we had a development version in Bitbucket's private repository. This is simply because we were just figuring out the content and all the other stuff so didn't want to have all that lorem ipsum to be viewed in public. Not that it would matter much, but for the cleaner outcome we decided to release the repository *as is*, as soon as the overall package would be ready.

Themes and sites before this version are forever resting in Bitbucket.

### What's ignored?

We have some stuff in [`.gitignore`](https://github.com/digitoimistodude/dude.fi/blob/master/.gitignore), although most of the lines are directly from [dudestack](https://github.com/digitoimistodude/dudestack).

- `.env`, in other words: credentials. All API keys, passwords and other sensitive information are hidden from the world and not included in the repository
- Fonts. We have purchased fonts for about 500 EUR so obviously those and lisences are ignored
- NPM building blocks. Dependencies should not be in upstream so those are ignored.
- Composer dependencies. WordPress and plugin installation files as well as custom-plugin dependencies are ignored in therepository.
- Paid plugins that do not have a composer repo (at least [WP-Rocket](https://wp-rocket.me))

## Features overview

- SASS, HTML, jQuery in the front end
- PHP, WordPress, Vue.js and WP-REST API the in back end
- Carefully selected fonts, responsive typography with viewport units with px fallback
- Built accessibility in mind
- All logos, icons and illustrations are SVGs + optimized with svgo

## Tools used

Dude.fi is based on:

- [air](https://github.com/digitoimistodude/air)
- [dudestack](https://github.com/digitoimistodude/dudestack)
- [marlin-vagrant](https://github.com/digitoimistodude/marlin-vagrant)
- [devpackages](https://github.com/digitoimistodude/devpackages)

## Building blocks

As usual, our site is built with today's technologies. Building blocks coming soon.

## Building instructions

Dude.fi is a personal views of the digital agency Dude, but if for some reason you'd want to contribute, here's the building instructions:

1. Clone/fork the repo
2. Run `composer install`
3. Run `npm install`
4. Run `gulp watch`
5. Make changes and send a pull request
