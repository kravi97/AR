# QR Code Setup Instructions

## Current Issue
Your existing QR code points to: `https://calm-panda-2bd6b0.netlify.app`
This goes to the main card page, not the AR experience.

## Solutions

### Option 1: Update Your QR Code (Recommended)
Generate a new QR code with one of these URLs:

#### For Auto-Redirect to AR:
```
https://calm-panda-2bd6b0.netlify.app/?ar=1
```
This will auto-detect mobile devices and redirect to AR experience.

#### For Direct AR Launch:
```
https://calm-panda-2bd6b0.netlify.app/ar.html
```
This goes directly to the AR camera page.

#### For Launch Screen:
```
https://calm-panda-2bd6b0.netlify.app/launch.html
```
Shows a nice landing page where users can choose AR or regular card view.

### Option 2: Use Launch Page as Default
Set `launch.html` as your default page in Netlify settings.

## How to Generate New QR Code

### Online Tools:
1. Visit: https://www.qr-code-generator.com/
2. Enter your chosen URL from above
3. Customize design if desired
4. Download and save to `assets/QR Images/`

### Or use this HTML generator:
Open `generate-qr.html` in your browser

## Recommended Flow

**For QR Code on Business Cards:**
```
QR Code → https://calm-panda-2bd6b0.netlify.app/launch.html
```

**For Direct AR Experience:**
```
QR Code → https://calm-panda-2bd6b0.netlify.app/ar.html
```

**For Auto-Redirect on Mobile:**
```
QR Code → https://calm-panda-2bd6b0.netlify.app/?ar=1
```

## Current Files Available

- `/` or `/index.html` - Main digital business card
- `/ar.html` - AR experience (requires camera)
- `/launch.html` - Landing page with options
- `/create-target.html` - Setup instructions
