---
title: "Introduction"
description: "A POSIX script that helps you find Youtube videos (without API) and opens/downloads them using mpv/youtube-dl"
lead: "A POSIX script that helps you find Youtube videos (without API) and opens/downloads them using mpv/youtube-dl"
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "prologue"
weight: 100
toc: true
---

<p align="center">
    <a> <img src=https://github.com/pystardust/ytfzf/raw/master/.assets/logo.png></a>
    <br />
    <br />
	<a href="https://github.com/pystardust/ytfzf/stargazers"><img src="https://img.shields.io/github/stars/pystardust/ytfzf?color=orange&logo=github&style=flat-square"></a>
	<a href="https://github.com/pystardust/ytfzf/graphs/contributors"><img src="https://img.shields.io/github/contributors/pystardust/ytfzf?style=flat-square"></a>
	<a href="https://github.com/pystardust/ytfzf/releases/tag/v1.0.0"><img src="https://img.shields.io/github/v/tag/pystardust/ytfzf?style=flat-square"> </a>
	<a href="https://github.com/pystardust/ytfzf/commits/master"><img src="https://img.shields.io/github/commit-activity/m/pystardust/ytfzf?color=green&style=flat-square"></a>
	<a href="https://discord.gg/TM4xy6J3"><img src="https://img.shields.io/discord/815609275644117022?color=yellow&logo=discord&style=flat-square" alt="Discord"></a>
    <br />
    <br />
	<hr>
</p>


<h1 align="center">
	This is a little showcase
</h1>
<p align="center">
<img src=https://github.com/pystardust/ytfzf/raw/master/.assets/ytfzf.gif width="100%">
</p>


## Fast installation

_This one-line installation does not support every OS, detail information for different OS can be found in the [here](../help/installation.html)_

```sh
curl -sL "https://raw.githubusercontent.com/pystardust/ytfzf/master/ytfzf" | sudo tee /usr/bin/ytfzf >/dev/null && sudo chmod 755 /usr/bin/ytfzf
```
<sup>*requires cURL</sup>

## Features

- Subscriptions
- Thumbnails
- History
- Download
- Format selection
- Queue multiple videos

## Update-Log

* We have now added Subscriptions which allows you to search between videos of subscribed channels easily
* Now ytfzf can queue videos using fzf multiselect option. Press tab to select a video. All the videos will be lined up in mpv. Use `>` and `<` to traverse them.
* Make continuous queries with `-s`
* You can preview video thumbnails now! Using Ueberzug. Inspired by [`fontpreview-ueberzug`](https://github.com/OliverLew/fontpreview-ueberzug).
* Stdin can be taken by using `ytfzf -`, for both fzf and external menu.
* Added MacOS support

## Todo

* [ ] Playlists
* [ ] More sites
* [x] Subscriptions
* [x] Thumbnails

## Bugs

* _dwm with swallow patch: Images don't render when looped (ie, option -l)_
- _If thumbnails are not working `.Xauthority` might be causing it. Try deleting `.Xauthority` and relogging._