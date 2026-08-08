# Responsive Split-Screen Login Page

A clean, modern, split-screen login page interface built using plain HTML5 and standard CSS3.

## Features

- Split-screen visual layout using CSS Flexbox.
- Full viewport height cover image using dynamic viewport units (`100dvh`).
- Native HTML5 form validation for email and password input fields.
- Interactive styling for state changes (hover states on buttons and links).
- Custom input styling with subtle shadow effects and clean typography.

## File Structure

```text
.
├── index.html   # Main markup containing the form and image structure
└── style.css    # Layout rules, typography, and visual styling
```

## Setup and Usage

1. Clone or download the repository files to your local system.
2. Open `index.html` directly in any web browser.

No build tools, preprocessors, or external dependencies are required to run this project.

## Code Overview

### Layout Design
The layout relies on a parent flex container (`.container`) split equally between two columns (`.left` and `.right`) using `flex-basis: 50%`:

- **Left Section (`.left`)**: Houses a side banner image set to `height: 100dvh` and `object-fit: cover` to ensure it fills the entire left column seamlessly without distorting the aspect ratio.
- **Right Section (`.right`)**: Contains the form container with centered typography and clean spacing.

### Form Validation
The form utilizes HTML attributes for basic browser-level validation:
- Email input requires a valid email structure (`type="email"`).
- Password input enforces a minimum length of 8 characters (`minlength="8"`).
