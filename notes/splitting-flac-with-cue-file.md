---
title: Splitting FLAC with CUE file
type: note
---

Make sure you have `cuebreakpoints` and `shnsplit` installed.

You will need a `.cue` file for the given FLAC.

```shell
cuebreakpoints [file].cue | shnsplit -o flac [file].flac
```
