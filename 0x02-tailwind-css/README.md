# 0x02 - Tailwind CSS
Tailwind CSS is a utility-first CSS framework that provides low-level utility classes to build custom designs directly in HTML. Unlike traditional CSS frameworks, Tailwind does not come with pre-designed components. Instead, it offers a set of utility classes that allow developers to create unique, responsive, and consistent designs without writing custom CSS.

### Why is Tailwind CSS Widely Used?

- **Customizable**: Tailwind allows developers to configure and extend its default design system to match their project's needs.
- **Responsive Design**: It includes built-in utilities for creating responsive layouts effortlessly.
- **Developer Productivity**: By using utility classes, developers can quickly prototype and build designs without switching between HTML and CSS files.
- **Consistency**: Ensures a consistent design language across the application.

## Project Objectives
The objectives of this project are to:

- Master Tailwind CSS Configuration
- Build Responsive Layouts
- Combine CSS Grid and Flexbox
- Design Aesthetically Pleasing Components
- Optimize for Professional Development

## How to Run

To run this project, ensure you have Tailwind CSS version 3.4 installed. Follow these steps:

1. **Install Dependencies**:
    Make sure you have Node.js and npm installed. Then, install Tailwind CSS by running:
    ```bash
    npm install -D tailwindcss
    npx tailwindcss init
    ```

2. **Build CSS**:
    Use the following command to generate your CSS file:
    ```bash
    npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
    ```

3. **Run the Project**:
    Open any of the HTML files in a browser.