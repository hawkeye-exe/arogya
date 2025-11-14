# Project Structure

This document outlines the professional directory structure of the Arogya project.

## Directory Overview

```
arogya-testing/
├── docs/                          # Project documentation
│   ├── CONTRIBUTING.md           # Contribution guidelines
│   ├── HACKATHON.md              # Hackathon-specific information
│   └── TEAM.md                   # Team information
│
├── public/                        # Public-facing files (web root)
│   ├── auth.html                 # Authentication page
│   ├── dashboard.html            # User dashboard
│   ├── index.html                # Main application entry point
│   ├── landing.html              # Landing page
│   ├── manifest.json             # PWA manifest
│   ├── service-worker.js         # Service worker for PWA
│   └── offline.html              # Offline fallback page
│
├── src/                          # Source files
│   ├── assets/                   # Static assets
│   │   ├── icons/                # Icon files
│   │   │   └── favicon/          # Favicon variants
│   │   └── images/               # Image files
│   │       └── profile-pics/     # User profile pictures
│   │
│   ├── css/                      # Stylesheets
│   │   ├── auth.css              # Authentication styles
│   │   ├── dashboard.css         # Dashboard styles
│   │   ├── index.css             # Main application styles
│   │   ├── landing.css           # Landing page styles
│   │   └── styles.css            # Global styles
│   │
│   └── js/                       # JavaScript files
│       ├── app.js                # Main application logic
│       ├── auth.js               # Authentication logic
│       ├── dashboard.js          # Dashboard functionality
│       ├── index.js              # Entry point scripts
│       ├── landing.js            # Landing page scripts
│       │
│       └── modules/              # Modular components
│           ├── appointment.js    # Appointment booking module
│           ├── config.js         # Configuration settings
│           ├── hospital.js       # Hospital data module
│           ├── pwa.js            # PWA functionality
│           ├── specialty.js      # Medical specialty module
│           ├── state.js          # State management
│           ├── symptoms.js       # Symptom checker module
│           ├── ui.js             # UI components
│           ├── verification.js   # Verification logic
│           └── voice.js          # Voice assistant module
│
├── .editorconfig                 # Editor configuration
├── .gitignore                    # Git ignore rules
├── .prettierrc                   # Prettier configuration
├── LICENSE                       # Project license
├── package.json                  # Node.js dependencies and scripts
└── README.md                     # Project overview

```

## Directory Descriptions

### `/docs`
Contains all project documentation including contribution guidelines, hackathon details, and team information.

### `/public`
The web root directory containing all HTML files and PWA-related files that are served to users. This is the entry point for the application.

### `/src`
Source code directory organized by file type:
- **`/assets`**: Static files like images and icons
- **`/css`**: All stylesheets organized by page/component
- **`/js`**: JavaScript files with modular architecture
  - **`/modules`**: Reusable JavaScript modules for specific functionality

### Root Files
- **`.editorconfig`**: Ensures consistent coding styles across editors
- **`.prettierrc`**: Code formatting configuration
- **`package.json`**: Project metadata and dependencies
- **`README.md`**: Main project documentation
- **`LICENSE`**: Project license information

## Development Guidelines

1. **HTML files** should be placed in `/public`
2. **CSS files** should be placed in `/src/css`
3. **JavaScript files** should be placed in `/src/js` or `/src/js/modules` for modular code
4. **Assets** (images, icons) should be placed in `/src/assets`
5. **Documentation** should be added to `/docs`

## Serving the Application

To serve the application locally:
```bash
npm start
# or for development with specific port
npm run dev
```

The application will be served from the `/public` directory.
