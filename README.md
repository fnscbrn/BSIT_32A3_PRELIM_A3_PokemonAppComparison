# Pokemon App File Comparison

## Overview
This document compares the files `script.js`, `styles.css`, and `test.html` from the root folder with the `pokemon-search` folder, which contains the React-based version of the application.

---

## 1. JavaScript Code (script.js vs. App.js)

| Feature       | `script.js` (Vanilla JS) | `App.js` (React) |
|--------------|----------------------|----------------------|
| **Framework** | Plain JavaScript | React.js |
| **State Management** | Uses `document.getElementById` to manipulate the DOM | Uses React's `useState` hook |
| **Event Handling** | `addEventListener` for form submission | React's `onSubmit` event inside JSX |
| **Fetching Data** | Uses `fetch()` inside an event listener | Uses an `async` function and updates state with `useState` |
| **Error Handling** | Displays errors inside a `<p>` tag | Uses React state (`setError`) to handle errors |
| **Rendering Data** | Manually updates `innerHTML` | Uses JSX to conditionally render Pokémon details |

📌 **Key Difference:**
- The vanilla JS version manipulates the DOM directly, while the React version follows a **component-based approach**, storing state and rendering data dynamically.

---

## 2. CSS Styles (styles.css vs. App.css & index.css)

| Feature       | `styles.css` (Vanilla) | `App.css` (React) |
|--------------|----------------------|----------------------|
| **File Name** | `styles.css` | `App.css` & `index.css` |
| **Styling Approach** | Global CSS applied to all elements | Component-scoped styling using `.App` class |
| **Main Differences** | Uses `#pokemon-details` for styling | Uses `.pokemon-details` class |
| **Text Color** | No specific styling for paragraphs | `p { color: #ff4500; }` is applied in React |

📌 **Key Difference:**
- Both styles are similar, but React’s version scopes styles using a `.App` class.

---

## 3. HTML vs. React JSX (test.html vs. App.js)

| Feature       | `test.html` (Vanilla) | `App.js` (React) |
|--------------|----------------------|----------------------|
| **Structure** | Plain HTML file with `<form>` and `<div>` | JSX inside a `return` statement |
| **Rendering** | Static HTML with JS modifying it | Dynamically rendered based on state |
| **Script Linking** | `<script src="script.js"></script>` | Imports JavaScript modules |

📌 **Key Difference:**
- In vanilla JS, elements are modified dynamically in the HTML file, whereas in React, everything is handled inside **one component (`App.js`)**.

---

## Conclusion
- The original version is a **simple HTML, CSS, and JavaScript project**.
- The `pokemon-search` folder contains a **React version of the same functionality**, with improved **state management and modular structure**.

