## Overview

Overview
This project is a simple Chrome extension that allows users to save and manage their favorite web pages directly from the browser. The extension captures URLs from the current tab or allows users to manually enter URLs, which are then saved and stored in the browser's local storage. Users can view and delete their saved URLs via a straightforward user interface.

##
## Features

Features
- Save the current tab's URL with a single click.
- Enter URLs manually to save.
- Display a list of saved URLs.
- Delete individual URLs or clear all saved URLs.
- Persist URLs in the browser's local storage to maintain the list across sessions.

##
## Installation Instructions

Installation Instructions
1. **Clone the repository**:
   ```bash
   git clone https://github.com/jonakapaj/chromeExtension.git
   ```

2. **Load the extension in Chrome**:
   - Open Chrome and go to `chrome://extensions/`.
   - Enable Developer mode by clicking the toggle switch in the top right corner.
   - Click the "Load unpacked" button.
   - Select the cloned repository directory.

3. **Start using the extension**:
   - You should now see the extension's icon in the Chrome toolbar.
   - Click the icon to open the extension popup and start saving URLs.

##
## Usage Examples

Usage Examples
1. **Saving the current tab's URL**:
   - Navigate to a website you want to save.
   - Click the extension icon in the toolbar.
   - Click the "Save Tab" button to save the current tab's URL.

2. **Manually adding a URL**:
   - Click the extension icon in the toolbar.
   - Enter the URL in the input field provided.
   - Click the "Save Input" button to add the URL to the list.

3. **Viewing saved URLs**:
   - Click the extension icon in the toolbar.
   - All saved URLs will be displayed in a list format.
   
4. **Deleting URLs**:
   - To delete an individual URL, click the delete button next to the respective URL.
   - To clear all saved URLs, use the "Delete All" button.

##
## Code Summary

Code Summary
### File: `chromeTake2.js`
This file contains the main logic for the Chrome extension, including event listeners, DOM manipulation, and local storage handling. Here's a breakdown of the key sections in the code:

- **Initialization**:
  - Retrieves existing leads from local storage and renders them if available.

- **Event Listeners**:
  - `tabBtn.addEventListener("click", ...)`: Event listener for saving the current tab's URL.
  - Other event listeners for input and delete buttons.

- **Utility Functions**:
  - `render(myLeads)`: Function to render the list of saved URLs.

##
## License

License
This project is licensed under the MIT License. See the `LICENSE` file for more information.