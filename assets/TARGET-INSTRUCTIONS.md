# How to Create targets.mind File

## Option 1: Use MindAR Compiler (Recommended)

1. Visit: https://hiukim.github.io/mind-ar-js-doc/tools/compile
2. Upload your business card image (PNG/JPG)
3. Click "Start" to compile
4. Download the generated `targets.mind` file
5. Place it in this folder (`assets/targets.mind`)

## Option 2: Use Command Line Compiler

```bash
npm install -g mind-ar-cli
mind-ar-compiler your-business-card-image.jpg
```

## Image Requirements

- Clear, high-quality image
- Good contrast and distinctive features
- Recommended size: 1024x1024 pixels
- Avoid plain white or highly reflective surfaces

## For Testing

Until you create the .mind file, the AR experience will use the pattern-based marker system as fallback.
