# Voyage Architect

Voyage Architect is a single-file holiday planner built as a static web app for easy hosting on GitHub Pages.

It helps a user:
- answer a short trip-planning survey
- build a multi-day itinerary using suggested activity cards
- view a trip dashboard with highlights, estimated costs, and packing progress
- run everything from one `index.html` file with no build step

## What it does

The app is designed to feel simple to open and easy to publish.

### Main features
- **Trip survey** with inputs for destination, trip length, budget, group size, activities, and pace
- **Planner view** to build each day of a trip using activity cards
- **Auto-build options** to quickly populate a day plan
- **Dashboard view** with:
  - trip summary
  - estimated budget breakdown
  - highlighted activities
  - packing list progress
  - useful destination search links
- **Single-file architecture** so it can be hosted easily on GitHub Pages
- **Responsive layout** for desktop and smaller screens
- **Glassmorphism-style UI** with a travel-themed background

## Project structure

This project is intentionally lightweight.

```text
/
├── index.html
└── README.md
```

Everything is contained inside `index.html`:
- HTML structure
- CSS styling
- JavaScript logic
- seed planner/activity data

## How to run locally

### Option 1: Open directly in your browser
1. Make sure the file is named **`index.html`**
2. Double-click it, or right-click and open it with your browser

### Option 2: Use VS Code Live Server
If you prefer, you can also run it with a local static server such as Live Server in VS Code.

## How to publish on GitHub Pages

1. Create a GitHub repository
2. Upload `index.html` and `README.md` to the **root** of the repo
3. Commit the files
4. Go to **Settings → Pages**
5. Under **Build and deployment**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** `main` (or your chosen branch)
   - **Folder:** `/ (root)`
6. Save
7. Open the GitHub Pages URL once it is generated

### Important note
If you click `index.html` inside the GitHub repository, GitHub will show the source code as text.
To see the actual website, use the **GitHub Pages site URL**.

## Tech stack

- HTML
- CSS
- Vanilla JavaScript

No frameworks, packages, or build tools are required.

## Current app flow

1. User completes the survey
2. User moves into the planner
3. User adds activities into day slots
4. User opens the dashboard to review the trip summary and estimates

## Notes

- The app currently uses built-in sample destination and activity data
- Recommendation links open search results related to the selected destination and activity ideas
- Since this is a static single-file app, it does not require a backend
- Data is not persisted to a database

## Possible future improvements

- Save/load trip plans
- Export itinerary to PDF
- Add more destinations and activity libraries
- Add images per destination or activity
- Add drag-and-drop planning
- Add currency selection
- Add dark/light theme switching
- Add local storage persistence

## Authoring note

This project was built as a lightweight, GitHub-friendly travel planner prototype with all core logic contained in one HTML file for easy editing and deployment.
