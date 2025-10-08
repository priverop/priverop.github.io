+++
title = 'My last contribution to SceneGate: Texim docs'
date = 2025-09-30T22:48:00+02:00
draft = false
toc = false
+++

## Introduction

Texim is a C# library, created by PleoNex (leader of [SceneGate](https://code.pleonex.dev/SceneGate/)), to work with images. It allows developers to transform custom formats into editable bitmap formats (.png, .jpg, .tiff...) and vice versa (importing a modified image to a custom format).

This is quite used in our fan-translation projects, where we need to export the game images (which are usually compressed and obfuscated) to editable formats.

## Learning curve

Being a newcomer of reverse engineering meant that I didn't have a solid foundation. I didn't know basic concepts as _color encodings_, _sprites_ or _image compressions_. 

This meant a lot of questioning and too much time spent on trial-and-error situations.

## Getting started guide

After finishing my 2025 goals for the [JUS project](/pages/jus/), I created a "getting started guide" for Texim. This tutorial will teach you the basics of the library through a practical example of a custom image format.

Check it out [here](https://code.pleonex.dev/SceneGate/Texim/docs/getting-started/tutorial.html).

## Next steps

My next goal will be to complete the fundamental documentation of the project. A basic introduction of the key concepts and what provides Texim for them.

For example: what are Sprites, what properties they usually have and how can we transform any custom sprite format to a one or more .png files.

Our only concern is that Texim has only been tested with NDS games, not even with 3DS images. That's why we still consider it a `proof of concept` and we haven't migrated it to [Yarhl](https://code.pleonex.dev/SceneGate/yarhl/) (the main framework of the team). So, it's quite possible that the documentation that I write will become useless in the future. 

But well, isn't the point of all these just having fun?