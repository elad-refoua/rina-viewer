# rina-viewer

A read-only viewer for the blinded Rina simulation transcripts (MENTI, Article 15).

The transcripts are **encrypted at rest in this repository** (AES-256-GCM, key derived from a
passphrase with PBKDF2-SHA256, 300k iterations). The page holds ciphertext only. Without the
passphrase there is nothing to read.

The viewer shows one conversation per screen, identified by a serial code (`SIM-0001` …
`SIM-0102`). Coding happens outside this site; the code on screen is what links a rating back to a
participant, and that mapping is held by Elad alone.

Nothing here identifies a participant: names, e-mail addresses, timestamps, the platform's own
scores and its post-simulation debrief were all excluded when the corpus was built.
