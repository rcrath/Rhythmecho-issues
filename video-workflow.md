# Video Production Workflow: DAW + OBS → YouTube

A step-by-step pipeline for recording and publishing RhythmEcho demo/walkthrough videos.

---

## Stage 1: DAW — Prepare the Audio

1. **Build the demo session**
   - Load RhythmEcho on a track with a representative source (guitar, drums, synth, etc.)
   - Set up a short loop or phrase that showcases the feature you're demonstrating
   - Dial in the plugin settings you want to show

2. **Routing for OBS capture**
   - Send your DAW master output to a virtual audio cable (e.g. VB-Audio Virtual Cable, Blackhole on Mac)
   - This lets OBS capture the DAW audio in sync with the screen

3. **Practice the moves**
   - Run through the demo a few times before recording
   - Keep it short — aim for 60–90 seconds of material per short

---

## Stage 2: OBS — Screen Capture

### Setup (one-time)

- **Video settings:** 1920×1080, 30 fps (or 60 fps if showing fast parameter changes)
- **Audio sources:**
  - Add the virtual cable as an audio input source
  - Mute your system desktop audio to avoid double-capture
- **Output:** Set recording path, format MP4 or MKV (MKV is safer — won't corrupt on crash)

### Per-session recording

1. Open your DAW session and get to the starting state
2. Switch to OBS, arm recording
3. Switch back to DAW — hit play
4. Record the full run-through, including any parameter tweaks you want to show
5. Stop DAW playback → switch to OBS → stop recording

**Tips:**
- Do multiple takes rather than trying to edit heavily — short takes are easy to redo
- Leave 2–3 seconds of silent/still time at the start and end for editing handles
- If a take has a good moment but a flubbed ending, note the timestamp and redo just that section

---

## Stage 3: Video Editing

### Ingest and sync

- Import the OBS recording (video + embedded audio) into your editor
- If the DAW audio sounds better than the OBS capture, export a clean mix from the DAW and replace the audio track (sync to the visual by waveform or a clap/click at the start)

### Edit for pacing

- Trim the handles
- Cut dead air and hesitations
- For shorts: keep the final cut under 60 seconds if targeting YouTube Shorts

### Polish

- Add a title card (plugin name + feature name) for the first 1–2 seconds
- Optional: zoom/crop to the relevant part of the UI when showing a specific control
- Add lower-third or caption if the feature name isn't obvious visually

### Export settings

| Setting | Value |
|---|---|
| Format | MP4 (H.264) |
| Resolution | 1920×1080 (or 1080×1920 for Shorts) |
| Bitrate | 8–12 Mbps for 1080p |
| Audio | AAC 192 kbps, stereo |
| Color space | Rec. 709 |

---

## Stage 4: YouTube Upload

### Before uploading

- Write the title, description, and tags while the video is exporting (don't do it cold at upload time)

### Title formula

```
RhythmEcho — [Feature Name] ([one-line hook])
```
Example: `RhythmEcho — Tap Tempo (the echo that breathes with you)`

### Description template

```
[One sentence on what this video shows.]

RhythmEcho is a VST3 delay plugin that follows your playing instead of locking to a project BPM.

🔗 Get it: [release link]
📖 Docs: [wiki link]
🐛 Issues / feedback: [issues link]

#RhythmEcho #VST #delay #plugin #[DAW name]
```

### Upload checklist

- [ ] Set visibility to **Unlisted** first — watch it back before publishing
- [ ] Add thumbnail (plugin screenshot + short title text, high contrast)
- [ ] Set category: **Music** or **Science & Technology**
- [ ] Add to a playlist (e.g. "RhythmEcho Shorts" or "Feature Walkthroughs")
- [ ] Enable **automatic chapters** or add manual timestamps in description
- [ ] Publish / schedule

---

## Quick-reference checklist per video

```
[ ] DAW session prepped and looping
[ ] Virtual cable routing confirmed
[ ] OBS recording settings correct
[ ] 2–3 takes recorded
[ ] Best take edited and exported
[ ] Title / description / tags written
[ ] Uploaded as Unlisted and reviewed
[ ] Thumbnail set
[ ] Published or scheduled
```
