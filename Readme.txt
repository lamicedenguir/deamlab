{\rtf1\ansi\ansicpg1252\cocoartf2759
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 How to view your web app in your local machine?\
\
To view `index.html` in your local browser, the simplest and most common method is to use a local development server. This ensures that all relative paths for images, CSS, and JavaScript load correctly, which a simple "double-click" on the file might sometimes fail to do.\
\
### Overview\
I will provide you with several options to view the file, ranging from the quickest "double-click" method to using a local server with tools already likely installed on your machine (like Python or Node.js). Using a local server is recommended for this specific file because it contains several linked resources (images, CSS, and JS) that might be blocked by browser security if opened directly via the `file://` protocol.\
\
### Key Options\
*   **Direct Open:** Open the file directly in the browser (Fastest).\
*   **Python Server:** Use Python's built-in module (Most common for developers).\
*   **VS Code Live Server:** Use an extension for real-time updates (Best workflow).\
\
### Implementation Steps\
1.  **Option 1: Direct File Access**\
    *   Find `index.html` in your macOS Finder.\
    *   Right-click the file, select **Open With**, and choose your preferred browser (Chrome, Safari, Firefox).\
2.  **Option 2: Using Python (Recommended)**\
    *   Open your terminal in the project root (`/Users/kands/Documents/GitHub/deamlab`).\
    *   Run the command: `python3 -m http.server 8000`.\
    *   Open your browser and navigate to `http://localhost:8000`.\
3.  **Option 3: Using VS Code Extension**\
    *   Install the "Live Server" extension in VS Code.\
    *   Click the "Go Live" button at the bottom right of the VS Code window while `index.html` is open.\
\
### Technical Considerations\
*   **Asset Paths:** The HTML file uses relative paths like `images/deamlab.png` and `css/sliderbanner.css`. These will resolve correctly as long as you start the server in the root directory.\
*   **Port Conflicts:** If port `8000` is already in use, you can change it to any other number (e.g., `python3 -m http.server 8080`).\
*   **Security:** Browsers restrict some features (like certain JavaScript modules or cross-origin requests) when using `file://` URLs. The local server avoids these restrictions.\
\
### Success Criteria\
*   The webpage loads in the browser.\
*   The University of Charlotte logo and DEAM Lab title are visible.\
*   Styles (CSS) and images are correctly displayed.\
\
Once you are ready, please toggle to **ACT MODE** and I can execute the command to start a server for you or confirm the file's presence.}