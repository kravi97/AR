# WebAR Business Card

A WebAR application that uses pattern recognition to display an interactive business card experience with video and contact information.

## Features

- 📷 **Image Tracking**: Uses your business card pattern for AR tracking
- 🎥 **Video Overlay**: Displays a transparent background video introduction
- 📝 **Key Offerings**: Shows 5 floating text elements with your services
- 🔗 **Social Links**: LinkedIn and Contact buttons
- 📱 **Mobile Optimized**: Responsive design for mobile devices

## Quick Start

### Method 1: Using Node.js (Recommended)

1. Make sure you have Node.js installed ([Download here](https://nodejs.org))
2. Double-click `start-server.bat` or run in terminal:
   ```bash
   node server.js
   ```
3. Open your browser and go to `http://localhost:8080`
4. Allow camera permissions when prompted
5. Point your camera at the business card pattern

### Method 2: Using any HTTP server

You can use any local HTTP server. For example:
- Python: `python -m http.server 8080`
- PHP: `php -S localhost:8080`
- Live Server extension in VS Code

## File Structure

```
/
├── index.html              # Main WebAR application
├── server.js              # Simple Node.js server
├── package.json           # Node.js configuration
├── start-server.bat       # Windows batch file to start server
└── assets/
    ├── pattern-Screenshot 2025-11-05 113126.patt  # AR pattern file
    └── vecteezy_15-seconds-countdown-timer-countdown-timer-15-second-15_29092810.webm  # Introduction video
```

## Customization

### Update Contact Information

In `index.html`, modify these functions:

```javascript
function openLinkedIn() {
    window.open('https://www.linkedin.com/in/yourprofile', '_blank');
}

function openContact() {
    window.open('mailto:contact@yourcompany.com?subject=Business Inquiry', '_blank');
}
```

### Change Key Offerings

Update the offerings in the HTML:

```html
<div class="offerings-container" id="offeringsContainer">
    <div class="offering-item">💼 Your Service 1</div>
    <div class="offering-item">📊 Your Service 2</div>
    <div class="offering-item">🚀 Your Service 3</div>
    <div class="offering-item">💡 Your Service 4</div>
    <div class="offering-item">🎯 Your Service 5</div>
</div>
```

### Replace Video

1. Add your video file to the `assets/` folder
2. Update the video source in `index.html`:
   ```html
   <video id="introVideo" 
          src="./assets/your-video-file.webm">
   ```

### Create New Pattern

1. Use the [AR.js Pattern Marker Generator](https://ar-js-org.github.io/AR.js/three.js/examples/marker-training/examples/generator.html)
2. Upload your business card image
3. Download the `.patt` file
4. Replace the existing pattern file in the `assets/` folder
5. Update the pattern URL in `index.html`

## Browser Compatibility

- ✅ Chrome (Android/Desktop)
- ✅ Safari (iOS/Desktop)
- ✅ Firefox (Android/Desktop)
- ✅ Edge (Desktop)

## Requirements

- Device with camera access
- HTTPS or localhost (for camera permissions)
- Modern browser with WebRTC support

## Troubleshooting

### Camera Not Working
- Ensure you're accessing via HTTPS or localhost
- Grant camera permissions when prompted
- Check if camera is being used by another application

### Pattern Not Detected
- Ensure good lighting conditions
- Hold the pattern steady and at appropriate distance
- Make sure the pattern is clearly visible and not tilted

### Video Not Playing
- Check video format (WebM recommended for web)
- Ensure video file is in the correct path
- Check browser console for error messages

## Technologies Used

- [A-Frame](https://aframe.io/) - Web VR/AR framework
- [AR.js](https://ar-js-org.github.io/AR.js-Docs/) - Augmented Reality for the web
- HTML5 Video API
- WebRTC for camera access

## License

MIT License - Feel free to modify and use for your projects!