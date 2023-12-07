# Eclipse
An all-black Google Chrome theme with dark grey highlighted tabs with guide how to make it.
# Creating the "Eclipse" Chrome Theme - Step-by-Step Guide

**Introduction:**
Welcome to the detailed guide on creating the "Eclipse" Chrome theme! This guide will walk you through each step, providing a clear understanding of the manifest file and how to customize the theme.

**Step 1: Prepare the Images:**
Begin by creating black and dark grey images for various theme elements. To maintain organization, create a new folder named "images" within your theme directory and place the images inside it.

1. Open Paint and go to "File" > "Image Properties."
2. Change the units to pixels and set the resolution to 3840 x 2160 for optimal 4K resolution.
3. Create a solid black image by selecting the "Edit Colors" option and setting the colour to #000000.
4. Save the black image as "#000000.png" in the "images" folder.
5. Similarly, create a dark grey image by setting the colour to #212121 and save it as "#212121.png" in the "images" folder.

**Step 2: Create a Manifest File:**
Create a file named `manifest.json` in your theme directory. Open it in a text editor and add the following code:

```json
{
  "manifest_version": 2,
  "name": "Eclipse",
  "version": "1.0",
  "description": "An all-black theme with dark grey highlighted tabs",
  "theme": {
    "images": {
      "theme_frame": "images/#000000.png",
      "theme_toolbar": "images/#000000.png",
      "theme_tab_background": "images/#212121.png",
      "theme_tab_foreground": "images/#000000.png",
      "theme_ntp_background": "images/#000000.png"
    },
    "colors": {
      "frame": [0, 0, 0],
      "toolbar": [0, 0, 0],
      "tab_text": [255, 255, 255],
      "bookmark_text": [255, 255, 255],
      "tab_background_text": [255, 255, 255]
    },
    "properties": {
      "ntp_background_alignment": "bottom"
    }
  }
}
```

**Understanding the Manifest:**
- `"name"`: The name of your theme.
- `"version"`: The version number.
- `"description"`: A brief description of your theme.

For the images section:
- `theme_frame`: Browser frame image.
- `theme_toolbar`: Browser toolbar image.
- `theme_tab_background`: Background image for tabs.
- `theme_tab_foreground`: Active tab image.
- `theme_ntp_background`: New Tab Page background image.

**Step 3: Load and Test:**
Open Chrome, go to `chrome://extensions/`, enable "Developer mode," and load your theme using "Load unpacked." Open a new tab to test your "Eclipse" theme.

Feel free to experiment and customize further to suit your preferences. Enjoy your personalised Chrome browsing experience!
