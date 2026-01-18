# Images Folder

This folder contains all images used in the portfolio website including profile picture, banner, projects, articles, reading list items, and learning resources.

## Critical Image Specifications

### Favicon
- **Current Issue**: Grainy appearance due to incorrect size
- **Required Size**: 32x32px and 16x16px versions
- **Recommended**: Create a 512x512px master, then scale down to 32x32px and 16x16px
- **Format**: PNG with transparency
- **File Size**: Under 10KB
- **Tool**: Use a favicon generator like [RealFaviconGenerator](https://realfavicongenerator.net/)
- **Filename**: `favicon.png` (or `favicon-32.png` and `favicon-16.png` for separate sizes)

### Profile Picture
- **Size**: 400x400px (1:1 square)
- **Display**: Shown as 200px circle in hero section
- **Max File Size**: 150KB for optimal clarity and speed
- **Format**: JPG (recommended), PNG, or WebP
- **Tips**: Professional headshot, well-lit, centered face, clean background
- **GIF Support**: Animated GIFs supported but keep under 500KB
- **Filename**: Set in `resources/profile.json`

### Banner Image
- **Size**: 1920x600px (3.2:1 aspect ratio)
- **Max File Size**: 300KB for optimal page load
- **Format**: JPG (photos), PNG (graphics), or WebP (best compression)
- **Filename**: Set in `resources/banner.json`

## Image Guidelines

### File Naming
- Use lowercase with hyphens for spaces (e.g., `my-project-image.jpg`)
- Be descriptive but concise
- Include the resource type if helpful (e.g., `project-mlops.jpg`, `book-ddia.jpg`)

### Image Specifications
- **Format**: JPG, PNG, or WebP
- **Recommended Size**: 600x400px (3:2 aspect ratio)
- **Maximum File Size**: 500KB for optimal loading
- **Optimization**: Compress images before adding them

### Adding Images

1. Add your image file to this folder
2. Update the corresponding JSON file in `/resources`
3. Set the `image` field to the filename (e.g., `"image": "project-mlops.jpg"`)
4. The `imageLabel` field will be used as fallback text if the image fails to load

### Example JSON Entry

```json
{
  "icon": "🤖",
  "image": "mlops-pipeline.jpg",
  "imageLabel": "MLOps Pipeline",
  "title": "End-to-End MLOps Pipeline",
  "description": "Production-ready MLOps infrastructure...",
  "link": "https://github.com/...",
  "linkText": "View on GitHub"
}
```

## Current Images

Currently, this folder is empty. Add images as needed for your portfolio items.

### Suggested Images to Add

- **Projects**: Screenshots or diagrams of your projects
- **Articles**: Featured images or relevant illustrations
- **Books**: Book covers (ensure you have rights to use them)
- **Videos**: Thumbnails (if not using YouTube embeds)
