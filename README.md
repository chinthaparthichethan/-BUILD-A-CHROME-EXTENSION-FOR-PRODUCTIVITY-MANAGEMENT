# -BUILD-A-CHROME-EXTENSION-FOR-PRODUCTIVITY-MANAGEMENT


##  *Name*: CHINTHAPARTHI CHETHAN  
## *Company*: CODTECH IT SOLUTIONS PVT. LTD  
## *ID*: CT12ITW  
## *Domain*: WEB DEVELOPMENT (CHROME EXTENSION)  
## *Duration*: JANUARY 5, 2025 – MARCH 5, 2025  
## *Mentor*: Neela Santhosh Kumar  

### Overview of the Project  
Project: **Productivity Chrome Extension**  
This project involves building a **Chrome Extension** designed to improve user productivity by providing features such as task management, website blocking, and quick notes. The extension integrates seamlessly with the browser and enhances user workflow efficiency.  

### Features  
The **Productivity Chrome Extension** includes the following features:  

- **Task Manager**: Users can create, edit, and delete tasks directly from the extension.  
- **Website Blocker**: Users can block distracting websites to stay focused.  
- **Quick Notes**: A simple notepad feature for jotting down important points.  
- **Dark Mode**: Option to toggle between light and dark themes.  
- **Storage Persistence**: Saves user preferences and data using Chrome's local storage API.  

### Prerequisites  
- **Google Chrome Browser** (Latest version)  
- **Basic Knowledge of HTML, CSS, and JavaScript**  
- **Chrome Developer Mode Enabled**  

### Step-by-Step Guide to Installing the Extension  
#### Step 1: Download the Extension Files  
- Clone or extract the project files into a local folder.  

#### Step 2: Enable Developer Mode in Chrome  
1. Open **Google Chrome**.  
2. Navigate to **chrome://extensions/**.  
3. Enable **Developer Mode** (toggle in the top-right corner).  

#### Step 3: Load the Extension  
1. Click **Load Unpacked**.  
2. Select the folder containing the extension files.  
3. The extension will be added to Chrome.  

#### Step 4: Using the Extension  
- Click the **Extension Icon** in the Chrome toolbar.  
- Use the interface to **add tasks, block sites, or take quick notes**.  

### Code Overview  
#### `manifest.json` (Manifest File)  
- Defines the extension's metadata, permissions, and background scripts.  
- Example:  
```json
{
  "manifest_version": 3,
  "name": "Productivity Extension",
  "version": "1.0",
  "description": "A Chrome extension for task management and website blocking.",
  "permissions": ["storage", "tabs", "activeTab"],
  "background": {
    "service_worker": "background.js"
  },
  "action": {
    "default_popup": "popup.html",
    "default_icon": "icon.png"
  }
}
```

#### `popup.html` (User Interface)  
- Contains the HTML structure for the extension’s pop-up window.  
- Displays **task input, blocked sites list, and notes section**.  

#### `popup.js` (Functionality)  
- Handles user interactions and updates stored data.  
- Uses `chrome.storage` API to save user preferences.  

#### `background.js` (Background Script)  
- Runs in the background and enforces website blocking rules.  
- Listens for tab updates and prevents access to blocked websites.  

### Conclusion  
This **Chrome Extension Project** provides a hands-on learning experience in **browser extensions, local storage, and JavaScript-based UI interactions**. It enhances productivity by helping users manage tasks, avoid distractions, and stay organized—all within their browser.  
