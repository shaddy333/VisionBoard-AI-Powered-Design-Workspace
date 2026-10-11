# VisionBoard

Browser-based design workspace: canvas, drag-and-drop, image uploads, text editing, layers, templates, zoom, undo/redo, a simulated AI assistant, project saving and responsive layout.

No build step and no dependencies. Open `index.html`, or serve the folder:

    npx serve .

## Structure

    index.html          page markup
    css/styles.css      theme tokens and layout
    js/state.js         state, history, rendering, layers and properties panels
    js/interactions.js  drag, resize, add, uploads, zoom, shortcuts
    js/templates.js     starter templates
    js/storage.js       save/open projects (localStorage), PNG export
    js/ui.js            theme toggle, mobile tabs
    js/assistant.js     rule-based assistant (swap in a real API here)
    js/main.js          startup
    assets/             static files

Scripts load in order as classic scripts and share globals, so keep the order in `index.html`.

## Deploy

Netlify or Vercel: connect the repo, leave the build command empty, publish directory `.`.
