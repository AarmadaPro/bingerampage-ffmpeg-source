# FFmpeg source for Binge Rampage

The Binge Rampage app ships an unmodified copy of **FFmpeg 6.1.1**, a separate program the app runs to cut and convert video.
FFmpeg is free software licensed under the **GNU General Public License version 3** (see `LICENSE`).
As the licence requires, this repository makes its complete source code available to everyone who receives the app.

## What is included

| Where the app runs | FFmpeg build shipped | Build notes |
|---|---|---|
| Windows (64-bit) | 6.1.1 "essentials" static build by gyan.dev | `builds/windows-x64-ffmpeg-6.1.1-gyan.dev-README.txt` (version, configuration, every enabled library and its version) |
| Mac (Intel) | 6.1.1 static build by evermeet.cx ("6.1.1-tessus") | `builds/mac-x64-ffmpeg-6.1.1-tessus-evermeet.cx-configuration.txt` |

Both binaries came to Binge Rampage through the npm package [ffmpeg-static](https://github.com/eugeneware/ffmpeg-static) (release `b6.1.1`) and are shipped **unchanged**.

## Source code

- **FFmpeg 6.1.1 source:** the `ffmpeg-6.1.1.tar.xz` file on this repository's [Releases page](../../releases)
  (identical to https://ffmpeg.org/releases/ffmpeg-6.1.1.tar.xz, SHA-256 `8684f4b00f94b85461884c3719382f1261f0d9eb3d59640a1f4ac0873616f968`,
  with FFmpeg's own signature file `ffmpeg-6.1.1.tar.xz.asc`).
- **Libraries built into those FFmpeg copies** (x264, x265, libass, freetype, fontconfig and others listed in the build notes) are
  each free software with their own public source; the build notes name every one and its version.

Questions or a request for any of this source on physical media: contact Binge Rampage through https://bingerampage.com.
This offer is valid for at least three years from the last time we distribute the app.

Binge Rampage's own code is a separate program that only runs FFmpeg; it is not covered by FFmpeg's licence.
