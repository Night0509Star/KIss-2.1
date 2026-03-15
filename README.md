🎸 KISS Tribute Web Page

🔗 Live Demo: [View on GitHack](https://raw.githack.com/Night0509Star/KIss-2.1/refs/heads/main/Kiss.html)

🎯 Overview

The KISS Tribute Web Page is a visually striking homage to the legendary rock band KISS, combining rock-and-roll aesthetics with modern web design. This project features a sunset-inspired gradient background, intricate band member mask elements, and a fully responsive layout, demonstrating both creativity and technical skill in HTML5 and CSS3.

This website is intended as a portfolio piece, showcasing proficiency in:

Responsive web design for multiple devices

Advanced CSS techniques, including pseudo-elements, clip-path, and animations

Interactive UI elements such as buttons, collapsibles, and smooth scrolling

Visual storytelling through layout, imagery, and typography

The project has been intensively tested, with daily sessions ranging from 20 to 50 tests per day. Testing often lasted from 9 AM to 3 PM, ensuring that features worked across desktop, laptop, tablet, and mobile devices. Continuous testing allowed precise error tracking and iterative improvement. While the site functions almost fully on mobile, minor tweaks remain to perfect the experience on smaller screens.

✨ Features
1. Sunset / Metal Gradient Background

A dramatic gradient inspired by KISS’s stage aesthetics and metal music:

body {
  background: linear-gradient(135deg, black, red, yellow, white);
  font-family: 'Metal Mania', cursive;
  color: #fff;
  margin: 0;
  padding: 0;
}

Sets the mood for the entire site

Works across all screen sizes

2. KISS Mask Circles

Each corner of the site displays a circle representing a band member:

Starchild

Demon

Spaceman

Catman

Masks are created using CSS pseudo-elements, clip-path, and animations:

.kiss-circle::before {
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  background: url('images/starchild-mask.png') no-repeat center/cover;
  border-radius: 50%;
  animation: pulse 2s infinite;
}

Circles scale proportionally on smaller screens

Hover effect: glow and subtle scale increase for interactive feedback

.kiss-circle:hover {
  transform: scale(1.05);
  box-shadow: 0 0 15px #ff0000, 0 0 25px #ffd700;
  transition: all 0.3s ease-in-out;
}
3. Responsive Layout

Built with CSS Grid and Flexbox to ensure content adapts naturally:

.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  padding: 20px;
}

Breakpoints:

Device	Width
Desktop	1400px+
Laptop	1024px
Tablet	768px
Mobile	480px and below
4. Interactive Buttons

KISS-inspired buttons with hover animations:

.button:hover {
  box-shadow: 0 0 10px #ff0000, 0 0 20px #ffcc00;
  transform: scale(1.05);
  transition: all 0.3s ease-in-out;
}

Enhances user engagement

Maintains the metal aesthetic

5. Collapsible Sections & Smooth Scrolling

Band member bios and song details are wrapped in <details> tags:

<details>
  <summary>Paul Stanley – Starchild</summary>
  <p>Lead singer and rhythm guitarist known for his iconic star makeup.</p>
</details>

Smooth scrolling for internal links:

html {
  scroll-behavior: smooth;
}
6. Custom Scrollbar

Enhances the modern aesthetic on desktop/laptop:

::-webkit-scrollbar {
  width: 12px;
}
::-webkit-scrollbar-track {
  background: #000;
}
::-webkit-scrollbar-thumb {
  background: #444;
  border-radius: 6px;
}
🧪 Development & Testing

Tested 20–50 times per day during development

Some days involved long sessions (9 AM – 3 PM), others shorter

Continuous testing helped locate errors in CSS and layout, ensuring responsive mask circles and interactive elements

Almost fully functional on mobile; small adjustments still needed

Works perfectly on desktop screens, with responsive layout and animations intact

🛠 Technologies Used

HTML5 – Structure and semantic content

CSS3 – Flexbox, Grid, pseudo-elements, clip-path, animations

Google Fonts – Metal Mania

Media Queries – Device responsiveness

CSS Variables – Easy theming (--accent-color, --border-color)

📂 File Structure
/project-root
│── index.html          # Main HTML file
│── style.css           # CSS styling
│── images/             # Band masks, gallery images, backgrounds
│── README.md           # Documentation
🚀 Installation

Clone or download the repository:

git clone https://github.com/Night0509Star/KIss-2.1.git

Open Kiss.html (or index.html) in any modern browser

Explore all features: gradient background, KISS masks, responsive layout, interactive buttons

🎨 Customization

Background Gradient: Modify in the body selector

Button Colors: Adjust CSS variables --accent-color and --border-color

KISS Mask Circles: Edit .kiss-circle pseudo-elements to tweak mask graphics or animations

⚖ License

Personal and educational use only

Free to modify code for learning purposes

KISS logos and images are copyright-protected

💻 Screenshots / Code Snippets
Example KISS Mask Circle (HTML)
<div class="kiss-circle" id="starchild"></div>
Responsive Grid Layout for Gallery
<div class="container gallery">
  <img src="images/kiss1.jpg" alt="KISS Concert">
  <img src="images/kiss2.jpg" alt="Band Members">
</div>
Smooth Scroll Navigation
<a href="#about">About</a>
<a href="#music">Music</a>
<a href="#gallery">Gallery</a>
