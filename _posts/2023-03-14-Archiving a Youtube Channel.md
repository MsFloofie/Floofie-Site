---
layout: default
title: Archiving a Youtube Channel
description: i'm depressed
---
---


# Backstory
---
On March 1st, 2023 at around 5:00 PM JST, Amano Pikamee [announced that she will be graduating from VOMs](https://www.youtube.com/watch?v=w_ejnHxTWrU). "Graduating" means that she is retiring her character and leaving [VOMS Project](https://voms.net/). Shortly after this announcement, many people (myself included) began to collaborate on archiving her channel before her termination date of March 31st. 2023 JST. On that date, all of her content will be deleted.

# yt-dlp
---
[yt-dlp](https://github.com/yt-dlp/yt-dlp) is a fork of youtube-dlc used to download YouTube videos, as well as download videos from [many other sites](https://github.com/yt-dlp/yt-dlp/blob/master/supportedsites.md). Taking up the difficult task of archiving her entire channel, this tool is an absolute godsend. For downloading, I used this command (replace [channel_URL] with the channel you want to archive):
<pre>yt-dlp [channel_URL]/videos -o '[%(upload_date)s] %(title)s.%(ext)s'
--embed-thumbnail --embed-metadata --download-archive [Name].txt
--merge-output-format mp4</pre>

Breakdown of the command above:
 <p> -o '[%(upload_date)s] %(title)s.%(ext)s': Changes the output name of the file to [Date] [Title].mp4</p>
 <p> --embed-thumbnail: Embed thumbnail in the video as cover art.</p>
 <p> --embed-metadata: Embed metadata to the video file.</p>
 <p> --download-archive: Download only videos not listed in the archive file. Record the IDs of all to prevent redownloading videos.</p>
 <p> --merge-output-format mp4: Merge thumbnail into the file and save as an MP4.</p><br>
Utilizing this command, I was able to download every uploaded video, livestream, membership stream, and short. This took about 14 days and totaled over 2.7TB of youtube content, and 907GB of her Twitch content. After her official graduation, I will be releasing a public torrent of her streams. All membership content will **NOT** be included and is for my personal archive only. 

You can find my torrent to her Twitch VOD archive on [nyaa.si](https://nyaa.si/view/1653264) or via [magnet URI](magnet:?xt=urn:btih:89ae4029e8c59711442aa69d004b4f83327012e1&dn=Twitch&tr=http%3a%2f%2fnyaa.tracker.wf%3a7777%2fannounce&tr=udp%3a%2f%2ftracker.opentrackr.org%3a1337%2fannounce&tr=udp%3a%2f%2fopen.stealth.si%3a80%2fannounce&tr=udp%3a%2f%2fopentracker.i2p.rocks%3a6969%2fannounce&tr=https%3a%2f%2fopentracker.i2p.rocks%3a443%2fannounce&tr=udp%3a%2f%2fexodus.desync.com%3a6969%2fannounce&tr=udp%3a%2f%2ftracker.openbittorrent.com%3a6969%2fannounce&tr=udp%3a%2f%2ftracker.torrent.eu.org%3a451%2fannounce).