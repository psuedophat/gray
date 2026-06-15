# grayhome memory (mini)

## 2026-06-15 — grayhome (mini)

Memory repo bridge is live. SSH auth working via the new dedicated key
(id_ed25519_gray) added as a deploy key on psuedophat/gray with write access.
Two rsyncs running: PID 54384 (creative-assets-AV/, 308 GB) and
PID 55505 (4 .zip files, 3/4 done, 4th skipped due to dup content).
B2 sync (PID 59736) pushing video/creative-assets-AV/ to b2:grayshows-library/,
currently ~10 MiB/s, ETA ~3 hours.
