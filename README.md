# Dev.Tube Contribution

DevTube is a free and open-source tech video hub, that is getting better every day thanks to **[❤️ amazing contributors](https://dev.tube/contributors).**

## Table of content
- [How to contribute a video](#how-to-contribute-a-video)
- [How to contribute a channel](#how-to-contribute-a-channel)
- [How to edit an existing video](#how-to-edit-an-existing-video)
- [How to remove a video](#how-to-remove-a-video)
- [How to add a speaker](#how-to-add-a-speaker)
- [How to improve dev.tube](#how-to-improve-devtube)

## How to contribute a video

All videos on DevTube are crawled automatically from a list of contributed channels, that live in this GitHub repository. You cannot contribute separate videos; you can only contribute channels or playlists. 

After your contribution is accepted, it takes a few days for videos do get on DevTube.

When videos appear online, you will see your karma increasing:

![karma up](/karma.png)

## How to contribute a channel

You can add a channel to **[channels.yml](https://github.com/watch-devtube/contrib/edit/master/channels.yml)**. DevTube automatically discovers playlists, so you don't need to contribute each playlist separately. 

> Warning: we don't accept channels with promotional and commercial videos. If your channel contains commercial videos, but you still want to share some of the technical videos, please, create a playlist and share that instead.

## How to edit an existing video

For each video there is a corresponding `<videoId>.yml` file automatically created in GitHub:

`https://github.com/watch-devtube/contrib/edit/master/videos/<videoId>.yml`

The structure of the video metadata looks like this:

```
speaker: 
    - name: Donald Trump
      twitter: realDonaldTrump
    - name: Elon Musk
      twitter: elonmusk
title: Title goes here
language: English
category: conference # or vlog
featured: true (you need to have enough karma points, see https://dev.tube/contributors)
recordingDate: 1444245407 
description: Some text goes here
```

* Please use spaces for formatting.
* Please, only add speaker information if it is a **real person**.

## How to remove a video

Just create an entry in **[ignored.yml](https://github.com/watch-devtube/contrib/edit/master/ignored.yml)** and explain why you think the video should be removed. 

## How to add a speaker

When a new video is being ingested, DevTube tries to automatically discover the speaker using a list of pre-defined speakers. You can add speakers to **[speakers.yml](https://github.com/watch-devtube/contrib/edit/master/speakers.yml).**

> When you add a new speaker, videos will be iterated through and tagged during the next crawling session. It might take up to a week. If you want to assign a speaker to videos faster, manually set the speaker on each video (see [How to edit an existing video](#how-to-edit-an-existing-video)).

## How to improve DevTube

If you have any ideas how DevTube can be improved, please create a new GitHub issue [here](https://github.com/watch-devtube/web/issues).
