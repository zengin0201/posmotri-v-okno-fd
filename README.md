https://github.com/zengin0201/posmotri-v-okno-fd.git
# 🪟 Look Out The Window: Interactive Video Explorer

A sophisticated video-streaming dashboard that allows users to explore cityscapes across different times of day. This project focuses on high-quality UI/UX implementation, custom form controls, and efficient DOM management using HTML5 templates.



## 🌟 Key Features

* **Dynamic Video Discovery:** Integrated with a REST API to fetch and filter city videos based on location and time of day.
* **Template-Based Rendering:** Utilizes `<template>` elements for performance-optimized UI updates, ensuring clean separation between HTML structure and JavaScript logic.
* **Custom UI Components:**
    * **Hand-crafted Form Controls:** Fully customized checkboxes and text fields with focus-visible states and accessible labels.
    * **Advanced Preloader:** A custom-built CSS animation ("Chasing Squares") for a premium loading experience.
* **Infinite Scroll / Pagination:** Implemented "Show More" functionality with asynchronous data fetching and dynamic list appending.
* **Stateful Video Player:** A custom synchronization system where clicking a card updates the main player without page reloads, maintaining active states on the UI.
* **Responsive Layout:** Built with a "Mobile-First" mindset, featuring a custom-styled scrollbar and fluid grid layouts.

## 🛠️ Tech Stack

* **Frontend:** Vanilla JavaScript (ES6+), HTML5 (Templates & Video API).
* **Styling:** CSS3 (Flexbox, BEM methodology, Advanced Pseudo-classes like `:has` and `:focus-visible`).
* **Animations:** Pure CSS `@keyframes` animations for loaders and transitions.
* **API Integration:** Practicum Video Content API.

## 🧠 Technical Deep Dive

### 🏗️ Efficient DOM Management
Instead of using `innerHTML`, which can be slow and insecure, this project clones `<template>` fragments. This approach is much closer to how React's Virtual DOM handles component creation, demonstrating a "framework-ready" mindset.

### 🎨 Custom Form Engineering
The search form uses `appearance: none` and custom pseudo-elements to create a unique visual style while maintaining 100% accessibility. I used the `:has()` selector to manage parent-level focus states—a modern CSS feature that eliminates the need for extra JS listeners.

### 🔄 Asynchronous Workflow
The application manages multiple loading states (preloaders for both the player and the list) and handles "404 Not Found" scenarios with a dedicated UI template, providing a robust user experience even when data is missing.

## 🚀 How to Run

1. Clone the repository.
2. Launch a local server (e.g., VS Code Live Server) to handle ES6 modules and local assets.
3. Start exploring cities!

---
*Developed by zengin(Alexey Borodin) — focusing on pixel-perfect layout and clean JavaScript architecture.*
