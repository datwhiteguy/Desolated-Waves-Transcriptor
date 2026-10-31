# Desolated Waves's Transcriptor

Alright, this is my transcriptor, **Desolated Transcriptor**. It's a local Windows app for turning audio & video into subtitles, with extra help for songs, lyrics, held notes & repeated lines.

I wanted something that gets most of the work done and makes the parts that need checking easier to deal with. It isn't 100% perfect, but it still hits above 90% accuracy.

**[Get version 1.4.0](https://github.com/datwhiteguy/Desolated-Waves-Transcriptor/releases/tag/v1.4.0)** · **[Download & setup steps](DOWNLOAD.md)** · **[User guide](https://github.com/datwhiteguy/Desolated-Waves-Transcriptor/releases/download/v1.4.0/User-Guide.pdf)**

## What it does

- Transcribes audio & video locally.
- Exports SRT subtitles, plain text & JSON.
- Uses supplied lyrics to help with song transcription and correction.
- Lets you correct imported SRT wording while keeping its existing cue timing.
- Offers Baseline, General, Country, Rap, Metal & EDM/dubstep profiles.
- Helps review possible mistakes, repeated words & held vocals.
- Saves projects so you can come back and finish reviewing them.

The engines, models & runtimes are bundled. You don't need Python, Shotcut or an account to use it. Extract the whole folder wherever you want, as long as the app can write there. Keep the folder's contents together when you move it.

## A few things to know

The app runs on **Windows 10/11 x64 with an AVX2-capable CPU**. The download is about **7.62 GB**, split into four parts for GitHub. [Read the download steps](DOWNLOAD.md) before grabbing it.

Baseline is the default. The other profiles are previews. Lyrics can help, but they don't prove what was actually sung. Holds, echoes, chopped vocals & heavy effects can still throw it off. Review flags are there to help; they won't catch every mistake. Give the captions a listen before calling them finished.

This build is unsigned. See the PDF for CPU/GPU settings, playback, review tools, moving the app & troubleshooting.

## What's uploaded

This repository holds the release documentation. The compiled app, PDF, checksums & separate third-party dependency sources are attached to [the release](https://github.com/datwhiteguy/Desolated-Waves-Transcriptor/releases/tag/v1.4.0). My application's own source code, personal recordings, lyrics, settings & saved projects aren't included.

Keep the included `Licenses` folder. The dependency source ZIP is there for those components' licenses; you don't need to install it. [More about the third-party files](THIRD-PARTY.md).

## Checks for 1.4.0

The packaged release passed 96 automated core/signal tests, nine packaged engine checks before and after ZIP extraction, three song-profile runs & cancellation testing. It was also checked after moving the app folder, and every packaged file matched its checksum.

Those checks cover the build and engine functions. They don't certify every lyric or timestamp. Interactive window operation, real speaker output & every possible PC/driver setup haven't been tested as part of these checks.
