# 99 Names of Allah - JSON with Timestamps

This repository contains a JSON file with **start timestamps** for the 99 Names of Allah (Arabic + transliteration).  
It allows developers to **highlight names while the audio is playing** in apps.

**Audio Source:** [YouTube Video](https://youtu.be/ta_tTZrarE0?si=denY02jVK4f1IhRA)  
**Note:** Convert this video to MP3 using any online tool or YouTube downloader, then use it in your app.

---

## Usage

Use with any audio player. Compute `end` as the start of the next name, or for the last name, use the total audio duration.

```swift
if currentTime >= name.start && currentTime < nextName.start {
    highlightedIndex = i
}
