# Tailwind User Panel

A modern, responsive user dashboard panel built with Tailwind CSS v4. Features a clean interface with Persian language support, sidebar navigation, and a fully customizable component-based architecture.


## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Project Structure](#project-structure)
- [Example Output](#example-output)
- [Author](#author)

## Overview

Tailwind User Panel is a production-ready dashboard template built with **Tailwind CSS v4.1.14** and vanilla HTML/CSS. It provides a responsive, accessible interface with modern UI patterns including a collapsible sidebar, navigation menu, and modular component structure. Perfect as a foundation for admin dashboards, user management systems, or project management applications.

## Features

- **Responsive Design** – Mobile-first approach with breakpoint-specific utilities
- **Sidebar Navigation** – Collapsible sidebar with smooth transitions
- **Tailwind CSS v4** – Latest Tailwind framework with optimized performance
- **Persian Language Support** – Full RTL support for Persian (Farsi) text
- **Accessible Components** – Semantic HTML and ARIA attributes
- **Dark Mode Ready** – Easy theme customization with CSS variables
- **Production Optimized** – Minified CSS, minimal dependencies
- **Component-Based** – Modular, reusable UI components

## Tech Stack

- **HTML5** – Semantic markup
- **CSS3** – Tailwind CSS v4.1.14 with modern utilities
- **Vanilla JavaScript** – No frameworks, lightweight interactivity
- **Node.js** – Optional build tooling (if using Tailwind CLI)

**Dependencies:**
- `tailwindcss@4.1.14` – Utility-first CSS framework

## Installation

### Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/awmiram/tailwind-user-panel.git
   cd tailwind-user-panel
   ```

2. **Open in browser:**
   ```bash
   # Simply open index.html in your browser
   open index.html
   
   # Or use a local server (recommended)
   python3 -m http.server 8000
   # Navigate to http://localhost:8000
   ```

### Development Setup

If you want to modify Tailwind configuration:

1. **Install Node.js** (v14 or higher)

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Build with Tailwind CLI:**
   ```bash
   npx tailwindcss -i ./src/input.css -o ./main.css --watch
   ```

4. **Start development server:**
   ```bash
   npm run dev
   ```

## Usage

### Basic Setup

The dashboard is a standalone HTML file. Include the CSS files in your project:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="main.css">
    <title>Dashboard</title>
</head>
<body>
    <div class="flex h-full">
        <!-- Sidebar -->
        <aside class="w-64 bg-indigo-800 text-indigo-100 p-4">
            <nav class="space-y-2">
                <a href="#" class="block px-4 py-2 rounded hover:bg-indigo-900">Dashboard</a>
                <a href="#" class="block px-4 py-2 rounded hover:bg-indigo-900">Teams</a>
                <a href="#" class="block px-4 py-2 rounded hover:bg-indigo-900">Projects</a>
            </nav>
        </aside>
        
        <!-- Main Content -->
        <main class="flex-1 p-8">
            <h1 class="text-2xl font-semibold">Welcome to Dashboard</h1>
        </main>
    </div>
</body>
</html>
```

### Customization

Edit `main.css` to customize colors, spacing, and component styles. Tailwind utilities are fully available:

```html
<!-- Using Tailwind utilities -->
<div class="bg-gradient-to-r from-indigo-500 to-purple-600 p-8 rounded-lg shadow-lg">
    <h2 class="text-white font-bold">Customizable Content</h2>
</div>
```

## Configuration

### Tailwind Configuration

If using the Tailwind CLI, modify `tailwind.config.js`:

```javascript
module.exports = {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {
      colors: {
        primary: '#4f46e5',
        secondary: '#7c3aed',
      },
    },
  },
  plugins: [],
}
```

### Environment Variables

No environment variables required for the standalone version. All configuration is handled through CSS utilities and HTML attributes.

### Customizing Colors

Update color variables in `main.css`:

```css
:root {
  --color-indigo-700: oklch(45.7% 0.24 277.023);
  --color-indigo-800: oklch(39.8% 0.195 277.366);
  --color-indigo-900: oklch(35.9% 0.144 278.697);
}
```

## Project Structure

```
tailwind-user-panel/
├── index.html          # Main dashboard HTML
├── main.css            # Compiled Tailwind CSS (v4.1.14)
├── style.css           # Custom styles (optional)
├── tailwind.config.js  # Tailwind configuration (optional)
├── package.json        # NPM dependencies
├── README.md           # This file
└── docs/
    └── components.md   # Component documentation
```

## Example Output

**Dashboard Layout:**
```
┌─────────────────────────────────────────────────────────────┐
│  Tailwind User Panel                                         │
├──────────┬──────────────────────────────────────────────────┤
│ Sidebar  │                                                  │
│ ▶ Dashboard                                                  │
│ ▶ Teams                                                      │
│ ▶ Projects                                                   │
│ ▶ Calendar                                                   │
│ ▶ Docs                                                       │
│ ▶ Reports                                                    │
│                                                              │
│ (Collapsible)  │  Main Content Area                          │
│                │  Responsive Grid                           │
│                │  • Card Components                         │
│                │  • Data Tables                             │
│                │  • Interactive Elements                    │
│                │                                            │
└────────────────┴──────────────────────────────────────────────┘
```

**Sample Navigation:**
```
Dashboard   Teams   Projects   Calendar   Docs   Reports
```

## Running Tests

Currently, this project uses manual testing. To verify:

1. **Open in multiple browsers:**
   ```bash
   # Test responsive design
   open -a "Google Chrome" index.html
   open -a Safari index.html
   ```

2. **Validate HTML:**
   ```bash
   npm run validate
   ```

3. **Check CSS performance:**
   ```bash
   npm run audit
   ```


## Author
 
GitHub: [@awmiram](https://github.com/awmiram)  

