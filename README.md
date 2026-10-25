# Chrome Freeze Demo

This repository intentionally contains a browser-breaking page. It is designed to stress CPU and memory by creating a huge number of DOM nodes, images, and blob objects in a loop.

## Purpose

This is only meant for learning, testing, and controlled local browser stress testing.

## Why it freezes

- A recursive animation loop keeps appending huge DOM fragments.
- It creates many images and blob URLs every frame.
- The browser spends all of its memory and CPU trying to render and manage the page.
- Modern browsers may become unresponsive or stop rendering.

## Important

Do not run this on production machines or real browsers you care about. Use only in a disposable or isolated environment.

## Fix

Remove the infinite render loop and the mass DOM creation code.
