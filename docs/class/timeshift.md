<tvh_include>inc/recording_contents</tvh_include>

---

## Overview

This tab is used to configure timeshift properties.

!['Timeshift Tab'](static/img/doc/recordings/timeshift.png)

---

## Recording from cache

With *Record from cache* enabled, every tuned channel keeps its own
cache of the last *Maximum period*, from the moment it was tuned. A
recording started after its programme began -- pressing record on what is
playing, typically -- then begins at the programme's start (less the
pre-recording padding), or as far back as the cache reaches, instead of
the moment it was requested. It works with every stream profile.

The cache holds the channel's stream as received, in the *Storage path*
(or in RAM with *RAM only*, bounded by *Maximum RAM size*). Normally it is
removed once nothing watches or records the channel any more. With *Keep
tuned channels* or a cache-only DVR warmup, the service can intentionally
remain tuned and its cache survives until that keepalive or warmup ends.

HTSP clients (Kodi) pausing, rewinding or skipping through live TV then use
that same cache instead of writing a buffer of their own: one cache per
channel, however many clients and recordings share it. A client paused
for longer than the cache holds goes on, when it resumes, from a little
after the oldest data still there.

---

## Buttons

<tvh_include>inc/buttons</tvh_include>

---
