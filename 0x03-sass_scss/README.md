# 0x03 - SASS & SCSS
SASS (`Syntactically Awesome Stylesheets`) and SCSS (`Sassy CSS`) are powerful extensions of CSS that add features like variables, nesting, and mixins, making it easier to write and maintain stylesheets.
SCSS is a superset of CSS, meaning all valid CSS is also valid SCSS.
SASS on the other hand gets rid of the curly braces and semicolons which are characteristic of CSS.

## Project Objectives
- Install and configure the SASS compiler in a development environment
- Understand the core philosophy of a CSS preprocessor and its advantages over vanilla CSS.
- Write and compile SASS (.scss) files into standard CSS.
- Apply core SASS features to solve common styling problems (variables, mixins, nesting)
## Installation of SCSS
To use SCSS, you need to install a preprocessor. Follow these steps:

1. Install Node.js and npm (Node Package Manager) if not already installed.
2. Install the `sass` package globally:
    ```bash
    npm install -g sass
    ```
3. Compile SCSS files to CSS:
    ```bash
    sass input.scss output.css
    ```

## Advantages of SCSS over Vanilla CSS
- **Variables**: Store reusable values like colors, fonts, and sizes.
- **Nesting**: Write styles in a hierarchical structure that mirrors HTML.
- **Mixins**: Reuse blocks of styles across multiple selectors.
- **Partials and Imports**: Break styles into smaller, manageable files.
- **Functions and Operators**: Perform calculations and manipulate values directly in stylesheets.

## Key Features of SCSS and SASS

### Variables
Variables allow you to store values for reuse throughout your stylesheets:

**SCSS:**
```scss
$primary-color: #3498db;
$font-stack: 'Roboto', sans-serif;

body {
  color: $primary-color;
  font-family: $font-stack;
}
```

**SASS:**
```sass
$primary-color: #3498db
$font-stack: 'Roboto', sans-serif

body
  color: $primary-color
  font-family: $font-stack
```

**Processed Output:**
```css
body {
  color: #3498db;
  font-family: 'Roboto', sans-serif;
}
```

### Mixins
Mixins let you define reusable blocks of styles:

**SCSS:**
```scss
@mixin flex-center {
  display: flex;
  justify-content: center;
  align-items: center;
}

.container {
  @include flex-center;
}
```

**SASS:**
```sass
@mixin flex-center
  display: flex
  justify-content: center
  align-items: center

.container
  @include flex-center
```

**Processed Output:**
```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

### Nesting
Nesting allows you to write styles in a way that reflects the structure of your HTML:

**SCSS:**
```scss
nav {
  ul {
     list-style: none;
     li {
        display: inline-block;
        a {
          text-decoration: none;
        }
     }
  }
}
```

**SASS:**
```sass
nav
  ul
    list-style: none
    li
      display: inline-block
      a
        text-decoration: none
```

**Processed Output:**
```css
nav ul {
  list-style: none;
}
nav ul li {
  display: inline-block;
}
nav ul li a {
  text-decoration: none;
}
```