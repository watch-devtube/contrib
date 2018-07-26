
# Dev.Tube Contribution Data

## Channel or playlist contribution guidelines

* Conference talks are accepted.
* Panel discussions are accepted.
* High quality video tutorials are accepted (only time-proven channels, with no aggressive marketing)
* No webinars.
* No commercial videos (product or company advertisement or hiring promotions).
* We do not add videos shorter than 5 minites. Short videos are automatically ignored.
* If your channel contains comercial videos, but you still want to share some of the technical videos, please, create a playlist and share that instead.

Channels and playlists can be added to [channels.yml](https://github.com/watch-devtube/contrib/edit/master/channels.yml).

## How to edit video metadata

* Please use spaces for formatting.
* Please, only add speaker information if it is a **real single person**. Collective names or organization accounts will not be accepted as a valid speaker metadata. We plan to implement multiple speakers per video at some point (follow up [here](https://github.com/watch-devtube/web/issues/50)). 

The structure of the video metadata looks like this:

```
tags:
    - tag1
    - tag2
speaker:
    name: Speaker full name
    twitter: SpeakerTwitterHandle (no @)
title: Title goes here
language: English
recordingDate: 1444245407 # 
description: Some text goes here #
```

## How to remove a video

If you want a video to be removed, create a new GitHub issue and explain why you think the video should be removed. In particular, we'd appreciate if you created issues for marketing videos.

## Video auto-tagging

In addition to editing video metadata, auto-tagging is supported. Auto-tagging takes place when video metadata is modified or a videos is ingested.

Contribute to auto-tagging by modifying [tags.yml](https://github.com/watch-devtube/contrib/edit/master/tags.yml)

## Speaker auto-discovery

When a new video is ingested, Dev.Tube tries to determine author's twitter account.

Contribute to speaker auto-discovery by modifying [speakers.yml](https://github.com/watch-devtube/contrib/edit/master/speakers.yml).

