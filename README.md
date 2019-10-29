# Canvas LMS for Franz
This is an un-official Franz recipe for Canvas LMS

### Installation
To install a new integration, download the integration folder e.g `canvas`.
1. Open the Franz Plugins folder on your machine (note that this dev directory may not exist yet, and you must create it -see below):
+ Mac: `~/Library/Application Support/Franz/recipes/dev/`
+ Windows: `%appdata%/Franz/recipes/dev/`
+ Linux: `~/.config/Franz/recipes/dev`
2. Copy the `canvas` folder into the `dev` plugins directory
3. Reload Franz

### To create the dev/ folder (if it does not exist)
1. Go to:
+ Mac: ~/Library/Application Support/Franz/recipes/
+ Windows: %appdata%/Franz/recipes/
+ Linux: ~/.config/Franz/recipes/
2. Create the folder as a new folder
3. Go back to the installation instructions

### Configuration for your Institution
Change `"serviceURL"` to the URL for your institution's Canvas LMS instance in `package.json`.
```
{
  "id": "Canvas",
  "name": "Canvas",
  "version": "1.0.0",
  "description": "Canvas LMS",
  "main": "index.js",
  "author": "Christiam Mendoza <your@email>",
  "license": "MIT",
  "config": {
    "serviceURL": "https://canvas.instructure.com",
    "hasNotificationSound": true
  }
}
```

### How to create your own Franz recipes:
* [Read the documentation](https://github.com/meetfranz/plugins)
