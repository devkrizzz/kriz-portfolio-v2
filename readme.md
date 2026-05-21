# Krizxter.mp4 — Cinematic Portfolio

A highly immersive, dark-themed, and cinematic portfolio website designed for **Kriz**, a content creator, editor, and filmmaker based in New Delhi. Built with a focus on motion, typography, and a seamless custom viewing experience.

## ✨ Features

* **Cinematic Dark Mode UI:** Deep blacks, subtle translucent borders, and a custom frosted-glass tracking cursor.
* **Custom HTML5 Video Player:** A fully custom-built video player that overrides native browser controls. Features include:
  * Custom play/pause overlay animations.
  * Interactive progress bar.
  * Dynamic timestamp timer (`0:00 / 0:00`).
  * Hover-to-expand volume slider & mute toggle.
  * Custom thumbnail (`poster`) support.
* **Dynamic Video Filtering:** A smooth, JavaScript-powered tab system to instantly filter video edits by category (All, Competition, Cinematic, Event, Personal).
* **Dedicated Contact Experience:** A standalone `contact.html` page featuring large, interactive cards with brand-specific neon hover glows (Instagram Pink, Discord Blurple, WhatsApp Green).
* **Scroll-Triggered Animations:** Clean `fade-up` and `reveal` animations powered by the Intersection Observer API for a premium, app-like feel.
* **Responsive CSS Grid:** A fluid layout that perfectly adapts from massive desktop monitors down to mobile screens (including side-by-side "wide" cards that smartly stack on phones).

## 🛠️ Technologies Used

* **HTML5:** Semantic structure and native media handling.
* **CSS3:** Custom animations, Flexbox/Grid layouts, custom scrollbars, and CSS variables for global theming.
* **JavaScript (Vanilla):** Custom video player logic, intersection observers, cursor tracking, and grid filtering. No heavy frameworks required.
* **Tailwind CSS (via CDN):** Used for rapid utility classes and layout scaffolding.
* **Google Fonts:** A curated cinematic typography stack utilizing *Bebas Neue*, *EB Garamond*, *Space Mono*, and *Poppins*.

## 📂 Project Structure

To ensure all images and videos load correctly, ensure your folder structure matches this layout:

```text
Kriz-Portfolio/
│
├── index.html           # Main portfolio page (Hero, About, Collabs, Work, Reviews)
├── contact.html         # Dedicated contact and social links page
├── README.md            # Project documentation
│
└── Assets/              # Main media directory
    ├── PFP/             
    │   └── kriz2.png    # Your profile picture for the About section
    ├── Videos/          
    │   └── *.mp4        # Your local high-quality video edits
    └── Thumbnails/      
        └── *.jpg        # Poster images for the video player before playback

```

## 🚀 How to Run Locally

Because this project uses vanilla web languages, no complex build tools, dependencies, or servers are required.

1. Clone or download this repository.
2. Ensure your videos and images are placed in the correct `Assets` subfolders.
3. Open `index.html` directly in any modern web browser (Chrome, Safari, Edge, Arc).
4. *(Optional but Recommended)* For the absolute best local testing experience with video files, run the folder using a local web server (like the "Live Server" extension in Visual Studio Code).

## ✏️ Customization Guide

### Updating Videos & Thumbnails

The portfolio is configured to play files directly from your computer for maximum quality and speed. To add or update a video, edit the `src` and `poster` attributes in the `<video>` tag within the `.custom-player` div in `index.html`:

```html
<video 
  src="/Assets/Videos/My_New_Edit.mp4" 
  playsinline 
  preload="metadata" 
  poster="/Assets/Thumbnails/My_New_Thumb.jpg">
</video>

```

### Updating Social Links

To update your Instagram, Discord, WhatsApp, or Email links, open `contact.html` (and the Hero section of `index.html`), locate the `href=""` attributes inside the `.contact-card` or `.btn-glow` elements, and replace the placeholder URLs:

```html
<a href="[https://wa.me/91XXXXXXXXXX](https://wa.me/91XXXXXXXXXX)" target="_blank" class="contact-card wa">
...
</a>

```

### Updating Reviews & Clients

The "Brands I've Worked With" and "Client Feedback" sections in `index.html` are hardcoded in standard HTML. Simply locate the `<section id="clients">` and `<section id="reviews">` tags in the code and edit the inner text to reflect your actual clients and testimonials.

## 📜 License & Author

Designed and developed by **Krizxter.mp4**.
*Jack of all trades, Master of none.*

```

```
