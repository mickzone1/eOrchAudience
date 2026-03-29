# Audio QR Code Generator

A simple web app for music educators to create QR codes for Google Drive audio files. Students can scan the QR code to listen to audio recordings.

## Features

- ✅ Add up to 5 Google Drive audio links
- ✅ Generate a single QR code for all tracks
- ✅ Simple player interface - just a play button
- ✅ Works on all devices (iOS, iPadOS, Android, Desktop)
- ✅ No backend required - pure HTML/JavaScript
- ✅ Educator-friendly interface

## Setup Instructions

### Step 1: Upload to GitHub

1. Create a new repository on GitHub (e.g., `eOrchAudience`)
2. Upload both `index.html` and `player.html` files
3. Or clone this repo and push to your GitHub

### Step 2: Enable GitHub Pages

1. Go to your repository **Settings**
2. Click on **Pages** in the left sidebar
3. Under "Source", select **main branch** (or master)
4. Click **Save**
5. Wait 1-2 minutes for your site to be published

### Step 3: Update the QR Code URL

In `index.html`, find this line (around line 245):
```javascript
const fullUrl = `https://yourusername.github.io/eOrchAudience/player.html#data=${btoa(JSON.stringify(validLinks))}`;
```

Replace `yourusername` with your actual GitHub username.

## How to Use

### For Educators (Creating QR Codes):

1. Open your GitHub Pages site (e.g., `https://yourusername.github.io/eOrchAudience/`)
2. Paste Google Drive audio links (up to 5)
3. Click "Generate QR Code"
4. Click "Save QR Code" to download the image
5. Print or share the QR code with students

### For Students (Listening):

1. Open camera app or QR scanner on device
2. Scan the QR code
3. Tap the big play button
4. Listen to the audio!

## Important: Google Drive Sharing Settings

For the audio to play properly:

1. Right-click your audio file in Google Drive
2. Click **Share**
3. Under "General access", select **Anyone with the link**
4. Set role to **Viewer**
5. Click **Done**

## Supported Audio Formats

- MP3
- WAV
- M4A
- OGG
- FLAC (browser dependent)

## Browser Compatibility

- ✅ Safari (iOS, iPadOS, macOS)
- ✅ Chrome (All platforms)
- ✅ Firefox
- ✅ Edge
- ✅ Samsung Internet

## Troubleshooting

**QR code doesn't work:**
- Make sure you updated the GitHub username in `index.html`
- Ensure GitHub Pages is enabled
- Wait a few minutes after pushing changes

**Audio won't play:**
- Check that the Google Drive file is set to "Anyone with the link can view"
- Make sure the link is a valid Google Drive audio file link
- Try opening the link directly in a browser first

**Can't save QR code:**
- Try long-pressing on the QR code image
- Or take a screenshot

## File Structure

```
eOrchAudience/
├── index.html      # Main page for creating QR codes
├── player.html     # Player page (shown when QR is scanned)
└── README.md       # This file
```

## License

Free to use for educational purposes.
