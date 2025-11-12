+++
title = 'Scenegate: creating a software ecosystem'
date = 2025-11-12T13:43:55+01:00
draft = false
toc = false
+++

## Tinke: the beginning

In 2011, Pleonex, one of the most important figures of NDS romhacking, created [Tinke](https://gbatemp.net/threads/tinke-0-7-2.303529/), _"a program to see, convert, and edit the files of NDS games"_.

The idea was to have just a single software for everything. Anybody could write plugins for their projects, in order to visualize their videogame custom formats, such as texts, images, music...

 _A single piece of software, to rule them all._

However, it was too hard to maintain, no CLI, no multi-platform...

After 5 years, the development stopped. That's when [SceneGate](https://code.pleonex.dev/SceneGate/) was born.

## The pieces of the puzzle

Sharing same architecture, API design, and language stack across its tools, SceneGate aims to create every single piece of software needed in every stage of a game localization project: researching, editing, testing and publishing.

Currently SceneGate gathers these tools:

- [Yarhl](https://code.pleonex.dev/SceneGate/Yarhl): the base framework . With it we can transform binary files to custom formats and vice versa. It also has a virtual file system.
- [Texim](https://code.pleonex.dev/SceneGate/Texim): an image library. It supports images, palettes, sprites, image compressions... 
- [Ekona](https://code.pleonex.dev/SceneGate/Ekona) / [Lemon](https://code.pleonex.dev/SceneGate/Lemon): NDS / 3DS rom management.
- [SceneGate](https://code.pleonex.dev/SceneGate/SceneGate): the only UI project. It uses the rest of the frameworks to analyze, visualize and convert any format of your game. 

The only thing left here is the plugins for the games, which is currently out of the scope of SceneGate. So right now you'll need to create your own project for your game, and implement your own formats and converters. 

> Note: Currently SceneGate is only focused on NDS/3DS, but anybody can create a library for their platform and integrate it with the rest of SG tools. 

## Continuous Deployment & Distribution

At Tradusquare, translations are managed through Weblate, which syncs changes directly to Git.

With SceneGate, anybody should be able to create a DevOps pipeline to get these files, transform them into the custom game formats, import them and even build a new beta to see the new changes. Automatically. A dream come true.

Moreover, with [Moxmi](https://code.pleonex.dev/pleonex/moxmi), the last addition, you have a CLI tool that automatically creates the patch for the translation/mod (even for different game regions and languages). It also has a multi-platform patcher with a user-friendly UI (or just CLI for the experts).

Even distributing your work can be automated.

## Wrap up

There are many generic tools that have been populating the rom hacking stack for a long time. These tools usually only work on Windows, they have no CLI and some of them... crash randomly...

Over time, we've seen many attempts of creating new generic tools, such as [Kuriimu](https://github.com/FanTranslatorsInternational/Kuriimu2), modernizing the rom hacking flow.

SceneGate is not inventing anything new, but it brings to the table a 360º approach for modding and game localization. We aim to build high quality tools following state of art best practices: 100% code coverage, integration tests, CI/CD, automated documentation, and getting started guides.

> Note: The whole project is developed by Pleonex. I am just a collaborator, and a big fan of how open-source keeps pushing the boundaries of technology.



