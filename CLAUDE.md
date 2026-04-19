# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

GitHub Pages site (linuxshark.github.io) — a collection of IT/VoIP/Cloud recipes. Static site using Jekyll with the `slate` theme, configured in `_config.yml`.

## Structure

- `README.md` — Landing page content (rendered as site index by GitHub Pages)
- `_config.yml` — Jekyll config (theme only)
- `recipes/` — Category index pages linking to external GitHub repos:
  - `asterisk/index.md` — Asterisk VoIP recipes
  - `linux/index.md` — Linux sysadmin recipes
  - `cloudcomputing/index.md` — AWS/OpenStack/K8s recipes

## Key Details

- No build step needed — GitHub Pages builds automatically on push to `master`
- All recipe content lives in separate GitHub repos; this site only links to them
- Content is plain Markdown, no front matter used
- To preview locally: `gem install jekyll bundler && bundle exec jekyll serve`

## Commit Convention

Prefix format from history: `[RL/ADD]:` for new content, `[RL/MOD]:` for modifications.
