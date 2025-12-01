## Tolet Bangla – Online To‑Let System

Modern, single‑page house rent listing UI built with HTML, Tailwind CSS (via CDN), and vanilla JavaScript. The project provides a Bangla‑first experience for browsing rental properties and posting new to‑let ads.

### Features
- **Landing page (`index.html`)**
  - **Hero image slider** with rotating property photos.
  - **Category filter** (Family, Bachelor, Office, Sublet, Hostel, Shop) that shows/hides featured cards dynamically.
  - **Featured properties** grid with example listings and quick contact buttons.
  - **Navigation bar** with links to Home, Property List, Add Post, Support, and Admin login.
  - **Bangla copy** throughout for a localized user experience.
- **Add Property page (`add_property.html`)**
  - **Animated video background** with glassmorphism style form card.
  - **Structured form** for category, beds, baths, balcony, drawing/dining arrangement, location, rent amount, rent type, and contact number.
  - **Photo upload widget** with custom “+” button and thumbnail previews.
  - **Client‑side validation** for minimum 3 photos, phone number format, and rent value.
  - **Preview modal** to review the post before final submission, plus a temporary success modal.
- **Admin & login placeholders**
  - `login.html` and `admin.html` are reserved for future admin authentication and dashboard functionality.

### Tech Stack
- **Frontend**: HTML5, Tailwind CSS via CDN, vanilla JavaScript.
- **Media/Assets**: Local PNG images (`0.png`–`5.png`) for the slider and a background video (`bgc.mp4`) for the add‑property page.
- **Deployment target**: Any static file server (no backend required for the current version).

### Folder Structure
- **`index.html`**: Main landing page with property discovery UI.
- **`add_property.html`**: Add‑property form with image uploads and preview.
- **`login.html`**: Admin login screen (UI only, no backend yet).
- **`admin.html`**: Placeholder for admin dashboard.
- **`0.png` – `5.png`**: Sample property images used in sliders/hero.
- **`bgc.mp4`**: Background video for the add‑property page.

### Getting Started (Local)
- **Prerequisites**: Any modern web browser (Chrome, Edge, Firefox, etc.). No build tools are required.
- **Run locally (simple way)**:
  - Download or clone this project into a folder on your machine.
  - Double‑click `index.html` to open it in your browser.
- **Run via a local server (recommended for consistent paths)**:
  - Use an extension like **Live Server** in VS Code, or run a simple HTTP server (e.g. `npx serve .` from the project root).
  - Open the served URL (for example `http://localhost:3000`) and navigate between `index.html` and `add_property.html`.

### Usage
- **Browse rentals**
  - Open `index.html`.
  - Use the **category chips** under “Browse by need” to filter properties.
- **Add a new property**
  - From `index.html`, click **Add Post** (or open `add_property.html` directly).
  - Fill in all required fields marked with `*`.
  - Upload **at least 3 photos** for the property.
  - Click **Post Property** to see the preview, then confirm to show the success animation.

> **Note:** In this version, data is not persisted to a real database or API. All interactions are frontend‑only demos suitable for UI/UX showcasing or as a starting point for a full‑stack implementation.

### Customization Ideas
- **Connect a backend** (Node/Express, Laravel, Django, etc.) to actually save and load property posts.
- **Add real authentication** for `login.html` and implement an `admin.html` dashboard for moderating posts.
- **Replace sample images/video** with your own property media.
- **Enhance validation** (multi‑language messages, stronger phone rules, etc.) and add map/location support.

### License
You may adapt or extend this UI for personal or educational projects. For commercial or large‑scale use, review and apply the license that best fits your needs.