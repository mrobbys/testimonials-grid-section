# Frontend Mentor - Testimonials Grid Section Solution

This is my solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). This project focuses on building a complex grid layout that showcases user testimonials, emphasizing responsive design and modern CSS practices using Tailwind CSS v4.

![Design Preview](./preview.jpg)

## Tech Stack

- **HTML5** (Semantic markup)
- **Tailwind CSS v4** (Modern styling via CDN)
- **CSS Custom Properties** (For specific brand colors)
- **Prettier** & **Prettier Plugin TailwindCSS** (Code formatting & class sorting)

## Project Overview

In this project, I built a responsive testimonial section that utilizes a multi-column grid system. The layout dynamically shifts from a single-column stack on mobile to a sophisticated 4-column grid on desktop. The main objective was to handle asymmetrical grid spanning (row and column spans) to match the professional design accurately.

### Key Features & Learnings

- **Semantic HTML Structure**:
  - Used `<main>` as the primary grid container for the entire section.
  - Implemented `<article>` for each testimonial card to ensure they are treated as independent, reusable pieces of content.
  - Structured user information (avatar, name, and status) using flexbox for better alignment within the cards.

- **Advanced CSS & Layout**:
  - **CSS Grid Mastery**: Leveraged Tailwind's grid utilities (`lg:grid-cols-4`) to build the layout. I specifically used `lg:col-span-2` for larger feature cards and `lg:row-span-2` for the tall vertical testimonial to create a balanced visual weight.
  - **Custom Color System**: Integrated the official style guide colors (Purple 500, Dark Blue, Grey 400, etc.) using CSS Variables (`:root`) and mapped them to custom utility classes like `.bege-purple` and `.teks-gray`.
  - **Layering & Positioning**: Used absolute positioning (`absolute`) and Z-index management (`z-10`) to place the quotation pattern image behind the text in the primary card, ensuring it doesn't interfere with readability.
  - **Responsive Breakpoints**: Followed a mobile-first approach, using a single-column layout for small screens and expanding to a full grid starting at the `lg` breakpoint.

- **Clean Code Practices**:
  - Configured **Prettier** with the **Tailwind CSS plugin** in the project environment to maintain consistent class ordering and clean code indentation automatically on save.
  - Used the latest **Tailwind CSS v4** CDN script for high-performance, browser-native styling without a complex build step.
