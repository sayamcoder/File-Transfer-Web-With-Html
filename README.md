# 🚀 QuickShare - Secure & Instant File Transfer

![Technology](https://img.shields.io/badge/Tech-HTML%20%7C%20CSS%20%7C%20JS-blueviolet)
![SEO Ready](https://img.shields.io/badge/SEO-Friendly-brightgreen)
![Deployment](https://img.shields.io/badge/Deployment-Single%20File-orange)

A modern, SEO-friendly, and privacy-focused file transfer website built entirely within a **single HTML file**. No server uploads, no sign-ups required. Share files directly from your browser with anyone, instantly.

---

### ✨ Key Features

-   **Modern & Responsive Design:**
    -   Sleek **Glassmorphism** interface for a premium look.
    -   **Dark/Light Mode** toggle to suit user preference, with settings saved in `localStorage`.
    -   Fully responsive layout for a seamless experience on desktop, tablets, and mobile devices.

-   **Effortless File Sharing:**
    -   Intuitive **Drag & Drop** file selection.
    -   Instantly generates a **Download Link** and a scannable **QR Code**.
    -   "Copy to Clipboard" button for easy link sharing.

-   **Privacy First (No Server Uploads):**
    -   **100% Client-Side:** Your files are never sent to or stored on a server.
    -   **Local Processing:** The `FileReader` API processes the file directly in your browser, ensuring your data remains private and secure.

-   **SEO-Friendly from the Ground Up:**
    -   Built with **Semantic HTML5** (`<main>`, `<section>`, `<footer>`).
    -   Optimized **meta tags** (title, description, keywords) for better search engine visibility.
    -   **JSON-LD Schema Markup** to provide structured data to Google, enhancing search result appearance.

-   **Zero Dependencies & Easy Deployment:**
    -   Everything is packed into a **single HTML file**. No need to manage external CSS or JS files.
    -   Extremely fast loading times.
    -   Deploy it easily on any static hosting service like GitHub Pages, Netlify, or Vercel.

### 🛠️ Technology Stack

-   **HTML5:** For the core structure and SEO-friendly semantic markup.
-   **CSS3:** For modern styling, including Flexbox, CSS Variables (for theming), transitions, and the glassmorphism effect.
-   **Vanilla JavaScript (ES6+):** For all functionality, including DOM manipulation, event handling, `FileReader` API for file processing, and `localStorage` for theme persistence.
-   **Embedded QR Code Library:** A minified, lightweight library is included directly in the script tag to generate QR codes without external dependencies.

### ⚙️ How It Works

This project provides a simulation of Peer-to-Peer (P2P) sharing using only client-side technologies. Here’s the technical breakdown:

1.  **File Selection:** The user selects a file from their device via drag-and-drop or the file input.
2.  **FileReader API:** JavaScript's `FileReader` API reads the file's contents locally in the user's browser.
3.  **Data URL Generation:** The file is converted into a **Data URL** (a Base64 encoded string). This URL contains all the file's data (e.g., `data:image/png;base64,iVBORw0KG...`).
4.  **Link and QR Code Creation:**
    -   The Data URL is assigned to the `href` attribute of a download button (`<a>` tag). The `download` attribute is used to tell the browser to download the content.
    -   A user-friendly "shareable link" is created (e.g., `your-page.html#filename.txt`) and a QR code is generated from it.
5.  **Sharing:** The user shares the download link or the QR code with a recipient. The recipient can then click the link or scan the code to download the file directly from the sender's browser session.

> **⚠️ Important Note:** Because the file is served directly from the sender's browser via the Data URL, the **sender must keep the browser tab open** until the recipient has finished downloading. Closing the tab will invalidate the link.

### 🚀 Getting Started & Deployment

Using or deploying QuickShare is incredibly simple.

#### To Use Locally:
1.  **Download:** Download the `index.html` file.
2.  **Open:** Open the `index.html` file in any modern web browser.
3.  **Share:** Start sharing files!

#### To Deploy (e.g., on GitHub Pages):
1.  **Fork this Repository:** Create a copy of this project in your GitHub account.
2.  **Go to Settings:** In your forked repository, go to `Settings > Pages`.
3.  **Select Branch:** Under "Build and deployment", select `main` as the source branch and `/ (root)` as the folder.
4.  **Save & Launch:** Click "Save". Your website will be live at `https://<your-username>.github.io/<repository-name>/` in a few minutes.

---

Made with ❤️ by Sayam
