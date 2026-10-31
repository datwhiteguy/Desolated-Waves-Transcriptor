# Third-party files

The app uses third-party engines, libraries & models. Their licenses and notices stay in the app's `Licenses` folder.

The separate [`Desolated-Transcriptor-1.4.0-Third-party-sources.zip`](https://github.com/datwhiteguy/Desolated-Waves-Transcriptor/releases/download/v1.4.0/Desolated-Transcriptor-1.4.0-Third-party-sources.zip) contains the native dependency sources & build instructions prepared for this release, including FFmpeg, Whisper.cpp, SDL2 & relevant runtime sources. It does **not** contain Desolated Transcriptor's own source code.

You don't need that ZIP to run the app. If you share the release, keep the corresponding dependency source ZIP available beside it and retain the included notices. FFmpeg is a shared LGPL build without the GPL/nonfree options. Its DLLs remain replaceable with compatible versions, under its license.

The full notices inside the package explain which terms apply to each component. This document doesn't add new license terms to the app.

The dependency source ZIP's SHA-256 is:

```text
2611f1c8862affb6822feb1981c398e67ad939155c31a80218b9bc8769313e90
```

See [FFmpeg's licensing page](https://ffmpeg.org/legal.html) and the license texts included with this release for the applicable details.
