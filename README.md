🚀 QuickShare - Secure & Instant File Transfer

![alt text](https://img.shields.io/badge/Tech-HTML%20%7C%20CSS%20%7C%20JS-blueviolet)

![alt text](https://img.shields.io/badge/SEO-Friendly-brightgreen)

![alt text](https://img.shields.io/badge/Deployment-Single%20File-orange)
A modern, SEO-friendly, and privacy-focused file transfer website built entirely within a single HTML file. No server uploads, no sign-ups required. Share files directly from your browser.
✨ Key Features
Modern & Responsive Design:
Sleek Glassmorphism interface.
Dark/Light Mode toggle to suit your preference.
Fully responsive layout for desktop, tablets, and mobile devices.
Effortless File Sharing:
Intuitive Drag & Drop file selection.
Instantly generates a Download Link and a QR Code.
Copy the link with a single click.
Privacy First:
No Server Uploads: Your files are never sent to a server. They are processed locally in your browser.
Client-Side Processing: The FileReader API creates a local Data URL, ensuring your data stays private.
SEO-Friendly:
Built with Semantic HTML5 (<main>, <section>, etc.).
Includes optimized meta tags (title, description, keywords).
JSON-LD Schema Markup for rich search engine results.
Zero Dependencies:
Everything is packed into a single HTML file. No external CSS or JS files to manage (the QR code library is embedded).
Extremely fast loading and easy to deploy.
📸 Screenshots
(You can add screenshots of your website here. It's a good practice to show both light and dark modes.)
Light Mode	Dark Mode

🛠️ Technology Stack
HTML5: For the core structure and SEO-friendly semantic markup.
CSS3: For modern styling, including Flexbox, Grid, CSS Variables (for theming), and animations.
Vanilla JavaScript: For all the functionality, including DOM manipulation, event handling, and file processing.
Embedded QR Code Library: A minified, lightweight library is included directly in the script tag to generate QR codes without external calls.

⚙️ How It Works
This project provides a simulation of Peer-to-Peer (P2P) sharing using only client-side technologies. Here's the magic:
File Selection: The user selects a file from their device.
FileReader API: JavaScript's FileReader API reads the file's contents locally.
Data URL Generation: The file is converted into a Data URL (a Base64 encoded string). This URL contains all the file's data.
Link and QR Code:
The Data URL is assigned to the href attribute of a download button (<a> tag). The download attribute tells the browser to download the content instead of navigating to it.
A "shareable link" is created (e.g., your-page.html#filename.txt). This link itself doesn't transfer the file but is used for the QR Code and for a user-friendly display.
A QR code is generated from this shareable link.
Sharing: The user shares the download link or the QR code with a recipient.
Important Note: Because the file is served directly from the sender's browser via the Data URL, the sender must keep the browser tab open until the recipient has finished downloading the file. Closing the tab will make the link invalid.

🚀 Getting Started
Using QuickShare is incredibly simple.
Download:
Download the index.html file from this repository.
Open:
Open the index.html file in any modern web browser (like Chrome, Firefox, or Edge).
Share:
Drag and drop a file onto the upload area or click to select one.
Copy the generated link or have the recipient scan the QR code.
Done!

📈 SEO Features Explained
This project was built with Search Engine Optimization in mind:
Meta Tags: The <head> section contains a descriptive <title>, <meta name="description">, and <meta name="keywords"> to help search engines understand the page's content.
Schema Markup (JSON-LD): A <script type="application/ld+json"> tag provides structured data to search engines, describing the site as a WebApplication. This can help in getting rich snippets in search results.
Semantic HTML: Using tags like <header>, <main>, <section>, and <footer> helps crawlers better parse the page structure and hierarchy.
Performance: Being a single file with no external requests makes the initial load time extremely fast, which is a positive ranking factor.

Made with ❤️ by Sayam
