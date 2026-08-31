# Alternating Tessellation Generator

A dynamic, interactive web tool that generates mathematically perfect tessellations of alternating tilted squares. Built with pure HTML, CSS, and JavaScript (SVG-based).

![Project Preview](link-to-your-screenshot.png) 
*(Note: Replace `link-to-your-screenshot.png` with a relative link to an image of the pattern in your repo, or remove this line).*

## 🌐 Live Preview

**[Click here to view the live demo](https://your-username.github.io/your-repo-name/)**

*(Note: Replace `your-username` and `your-repo-name` with your actual GitHub details and ensure GitHub Pages is enabled in your repository settings).*

## 🌟 Overview

This project creates an endless geometric pattern where squares tilt alternately clockwise and counter-clockwise, perfectly touching each other at their vertices. Built to visualize geometric principles, it allows users to adjust the rotation angle and grid density in real-time, rendering the shapes as clean, scalable vector graphics (SVG).

## 🧮 The Mathematics

To ensure the squares touch perfectly at their vertices **at any angle**, the code relies on precise geometric calculations:

- **Base Shape:** A square with a side length of `1`.
- **Center-to-Vertex Radius (`r`):** The distance from the center of the square to any of its four corners is `r = (side * √2) / 2`.
- **Grid Pitch (`p`):** The distance between the centers of adjacent squares is calculated using the formula `p = 2 * r * cos(θ)`, where `θ` is the chosen rotation angle. This ensures the tips of the squares meet flawlessly.
- **Alternating Rotation:** The grid uses a checkerboard logic `(i + j) % 2`. If the sum is even, the square rotates clockwise (`+θ`); if odd, it rotates counter-clockwise (`-θ`).

## ✨ Features

- **Interactive Angle Slider:** Adjust the rotation angle dynamically between **0° and 45°**. The squares will always mathematically adjust to stay touching at their vertices.
- **Adjustable Grid Density:** Change the number of squares per row/column from 2 to 15.
- **Custom Colors:** Choose separate colors for the clockwise and counter-clockwise squares to easily visualize the alternating pattern.
- **SVG Rendering:** Uses the Scalable Vector Graphics (SVG) format, ensuring the pattern is crisp at any screen resolution.
- **Downloadable:** Export your current custom pattern directly as an `.svg` file.

## 🚀 Getting Started

### Prerequisites
You do not need to install any dependencies, package managers, or run a local server. The project is entirely front-end and runs completely in the browser.

### Installation & Usage
1. **Clone the repository** (or download the `index.html` file):
   ```bash
   git clone https://github.com/your-username/your-repo-name.git