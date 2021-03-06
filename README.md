# mtlynch.io

[![Build
Status](https://travis-ci.org/mtlynch/mtlynch.io.svg?branch=master)](https://travis-ci.org/mtlynch/mtlynch.io)

## Overview

This is the source for https://mtlynch.io/.

## Code style guides

New code should adhere to the appropriate Google Style guide for the given language:

* [HTML/CSS](https://google.github.io/styleguide/htmlcssguide.html)
* [JavaScript](https://google.github.io/styleguide/jsguide.html)

## Dev / prod consistency

`script/_serve_dev.sh` builds the site in dev mode and starts a web server on http://localhost:4000.

`.travis.yml` builds the site in production mode and pushes the static files to Firebase.

Dev and prod configurations should be as similar as possible. Any change in dev should also be made to prod and vice versa, except for features we deliberately make different for dev and prod (e.g. removing GA tag from dev, removing jekyll-admin from prod).

## Theme

This blog uses the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme.

Where possible, avoid duplicating code from the theme. Sometimes this will be unavoidable. The blog currently duplicates theme code in several places, but we seek to minimize this duplication.

## Pull requests

### Merge conflicts

If a PR has merge conflicts with the main repo's `master` branch, rebase the PR onto `master`. Do not include merge commits in a PR.

### Pull request style

PRs should have a descriptive one-line summary to explain the change. The PR description should add any additional required context or explanation for the change. For simple or obvious PRs, a PR description is not required.

If the PR fixes an issue, include the text "Fixes #XX" in the PR description, where `XX` is the [repo issue](https://github.com/mtlynch/mtlynch.io/issues) number. This allows Github to cross-reference between PRs and issues.

## Prose style guide

### Headings

* Headings start with `<h1>` (single hash in Markdown).
* Headings use sentence-style capitalization (only first word is capitalized).
* Headings do not have trailing punctuation.

### Point of view

* Author is first-person singular (I).
* Reader is second-person singular (you).

### Readers

* Readers of the blog are collectively referred ot as "readers" or "visitors."
  * Readers are not referred to as "users" and should never be described as "traffic."

### Numbers

* For 1-9, spell out the number.
* For all other numbers, use numerals.

### Names

* reddit is written all lowercase.

### Oxford comma

* Always use an Oxford comma.
