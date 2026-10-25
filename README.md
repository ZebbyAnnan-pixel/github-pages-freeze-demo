# GitHub Pages Freeze Demo

This repository intentionally contains a broken GitHub Pages setup that causes the browser to get stuck in a redirect loop.

## Why it freezes

- The page immediately redirects to itself.
- A JavaScript timer keeps redirecting again and again.
- The browser keeps reloading the same page forever.
- This uses CPU and memory until Chrome becomes unresponsive.

## How to test

1. Create a GitHub repository.
2. Push this code to the `main` branch.
3. Go to Settings → Pages.
4. Deploy from the `main` branch.
5. Open the GitHub Pages URL.
6. Chrome may freeze or become extremely slow.

## Fix

Remove both the meta-refresh and the JavaScript redirect loop.
