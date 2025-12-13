# Images Directory

Create an `images` folder in your repository root and add the following images:

## Required Images

### Profile and Branding
- `profile.jpg` - Your professional headshot (recommended: 560×560px)
- `institution-logo.png` - Your institution's logo (recommended: 240×120px with transparent background)

### Research Spotlight Images (for Home page)
- `research1.jpg` - Featured research project 1 (recommended: 600×400px)
- `research2.jpg` - Featured research project 2 (recommended: 600×400px)
- `research3.jpg` - Featured research project 3 (recommended: 600×400px)

### Publication Thumbnails (for Publications page)

#### 2025
- `pub2025-1.jpg` - Publication thumbnail (recommended: 400×300px)
- `pub2025-2.jpg` - Publication thumbnail (recommended: 400×300px)

#### 2024
- `pub2024-1.jpg` - Publication thumbnail (recommended: 400×300px)
- `pub2024-2.jpg` - Publication thumbnail (recommended: 400×300px)
- `pub2024-3.jpg` - Publication thumbnail (recommended: 400×300px)

#### 2023
- `pub2023-1.jpg` - Publication thumbnail (recommended: 400×300px)

#### Preprints
- `preprint1.jpg` - Preprint thumbnail (recommended: 400×300px)

## Image Guidelines

### File Formats
- **Photos**: Use JPEG (.jpg) for photographs and complex images
- **Logos/Graphics**: Use PNG (.png) for logos, icons, and graphics with transparency
- **Simple Graphics**: Consider SVG (.svg) for vector graphics and simple illustrations

### Optimization
- Compress images to reduce file size
- Use online tools like:
  - TinyPNG (https://tinypng.com/)
  - Squoosh (https://squoosh.app/)
  - ImageOptim (for Mac)

### Naming Convention
- Use lowercase letters
- Use hyphens instead of spaces
- Be descriptive but concise
- Examples:
  - ✅ `profile.jpg`
  - ✅ `federated-learning-diagram.jpg`
  - ❌ `IMG_1234.jpg`
  - ❌ `My Photo 2024.jpg`

### Accessibility
- Ensure good contrast for text overlays
- Use descriptive alt text in HTML
- Test images on both light and dark backgrounds

## How to Add Images

### Method 1: GitHub Web Interface
1. Navigate to your repository on GitHub
2. Click "Add file" → "Upload files"
3. Drag and drop your images
4. Create `images` folder if it doesn't exist
5. Commit changes

### Method 2: Git Command Line
```bash
# Create images directory
mkdir images

# Copy your images into the directory
cp /path/to/your/images/* images/

# Add to git
git add images/
git commit -m "Add website images"
git push
```

### Method 3: GitHub Desktop
1. Copy images to `images` folder in your local repository
2. Open GitHub Desktop
3. Review changes
4. Write commit message
5. Push to GitHub

## Placeholder Images

If you don't have images yet, you can use placeholder services:
- https://placehold.co/ (e.g., https://placehold.co/600x400)
- https://picsum.photos/ (e.g., https://picsum.photos/600/400)
- https://via.placeholder.com/ (e.g., https://via.placeholder.com/600x400)

Example in HTML:
```html
<img src="https://placehold.co/600x400" alt="Placeholder">
```

## Common Issues

### Image Not Showing
- Check the file path is correct
- Ensure image is in the `images` folder
- Verify filename matches exactly (case-sensitive)
- Confirm image was committed and pushed to GitHub

### Slow Loading
- Compress images before uploading
- Use appropriate image dimensions
- Consider using WebP format for better compression

### Copyright
- Only use images you have rights to
- For publications, use your own figures or get permission
- Consider creating simple graphics with Canva or Figma
