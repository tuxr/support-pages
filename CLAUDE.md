# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static support pages for the **Simple Macro** iOS app, hosted via GitHub Pages at `https://tuxr.github.io/support-pages/`.

- `index.html` — Support & FAQ page
- `privacy.html` — Privacy Policy

## Deployment

Push to `main` to deploy. GitHub Pages serves the site automatically — no build step, no static site generator. The files are plain HTML with inline CSS.

## Architecture

Both pages are self-contained single-file HTML documents with inline `<style>` blocks. They share the same design system (Apple-style cards, gradient header, consistent typography via `-apple-system` font stack). When editing styles, keep both files in sync.

## Key Conventions

- The privacy policy effective date (bottom of `privacy.html`) must be updated whenever the policy content changes.
- Privacy disclosures should describe data flows generically (e.g., "cloud service" not specific vendor/model names) so implementation changes don't require policy updates.
- FAQ entries in `index.html` should mirror features disclosed in `privacy.html` where relevant.
