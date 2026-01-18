# Portfolio Resources

This folder contains all the content data for the portfolio website in JSON format. This modular structure makes it easy to update, add, remove, or reorder content without modifying the main HTML file.

## Files

### `projects.json`
Contains all project cards displayed in the Projects section.

**Fields:**
- `icon`: Emoji icon for the card
- `image`: (Optional) Filename of image in `/images` folder (e.g., "project-screenshot.jpg")
- `imageLabel`: Text label for the card image placeholder (used when no image is provided)
- `title`: Project title
- `description`: Brief description of the project
- `link`: URL to the project (usually GitHub)
- `linkText`: Text for the link button

> **Note**: If both `image` and `imageLabel` are provided, the image will be displayed. If the image fails to load, the imageLabel text will be shown as fallback.

### `articles.json`
Contains all article cards displayed in the Articles section.

**Fields:**
- `icon`: Emoji icon for the card
- `imageLabel`: Text label for the card image placeholder
- `title`: Article title
- `description`: Brief description of the article
- `link`: URL to the article
- `linkText`: Text for the link button

### `reading-list.json`
Contains all book recommendations displayed in the Reading List section.

**Fields:**
- `icon`: Emoji icon for the card
- `imageLabel`: Text label for the card image placeholder
- `title`: Book title
- `description`: Author and brief description
- `link`: URL to learn more about the book
- `linkText`: Text for the link button

### `learning-resources.json`
Contains all video resources (Dave Rensin and others) displayed in the Learning Resources section.

**Fields:**
- `icon`: Emoji icon for the card
- `hasEmbed`: Boolean indicating if the video should be embedded
- `embedUrl`: YouTube embed URL (if hasEmbed is true)
- `embedTitle`: Title for the iframe (if hasEmbed is true)
- `imageLabel`: Text label for the card image placeholder (if hasEmbed is false)
- `title`: Video title
- `description`: Brief description of the video content
- `link`: Direct YouTube URL
- `linkText`: Text for the link button

## How to Update Content

### Adding a New Item
1. Open the appropriate JSON file
2. Add a new object to the array with all required fields
3. Save the file
4. Refresh the website to see changes

### Removing an Item
1. Open the appropriate JSON file
2. Delete the entire object for the item you want to remove
3. Save the file
4. Refresh the website to see changes

### Reordering Items
1. Open the appropriate JSON file
2. Cut and paste objects in the array to change their order
3. Items will appear on the website in the same order as in the JSON array
4. Save the file
5. Refresh the website to see changes

### Updating an Item
1. Open the appropriate JSON file
2. Find the object you want to update
3. Modify the fields as needed
4. Save the file
5. Refresh the website to see changes

## Example: Adding a New Project

```json
{
  "icon": "🚀",
  "imageLabel": "New Technology",
  "title": "My New Project",
  "description": "A brief description of what this project does and why it's interesting.",
  "link": "https://github.com/username/project",
  "linkText": "View on GitHub"
}
```

## Example: Adding a New Learning Resource with Embedded Video

```json
{
  "icon": "🎥",
  "hasEmbed": true,
  "embedUrl": "https://www.youtube.com/embed/VIDEO_ID",
  "embedTitle": "Video Title for Accessibility",
  "title": "Video Title",
  "description": "Description of what the video covers and who presents it.",
  "link": "https://www.youtube.com/watch?v=VIDEO_ID",
  "linkText": "Watch on YouTube"
}
```

## Notes

- All JSON files must be valid JSON format
- Make sure to include commas between objects in the array
- Don't add a comma after the last object in an array
- Use double quotes for all strings
- Test your changes locally before deploying
