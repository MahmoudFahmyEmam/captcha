
# Category-Based CAPTCHA

A dynamic, interactive CAPTCHA implementation that challenges users to select images matching a randomly chosen category. This project is designed to enhance user verification through visual recognition.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)
- [Dependencies](#dependencies)
- [Future Enhancements](#future-enhancements)
- [License](#license)

## Introduction

The **Category-Based CAPTCHA** is a web-based verification tool that uses image recognition tasks to ensure that users are human. By selecting images matching a specified category, users prove their identity while engaging in a user-friendly activity.

## Features

- Randomized image grid with dynamic target categories.
- Intuitive visual selection interface.
- Instant feedback for user submissions.
- Automatic CAPTCHA refresh on completion.
- Lightweight and browser-compatible design.

## Installation

1. **Download the Project**:
   Clone or download this repository to your local machine.
   ```bash
   git clone https://github.com/MahmoudFahmyEmam/captcha
   ```

2. **Prepare the Environment**:
   - Place the project files in your web server's root directory.
   - Create an `images` folder in the same directory as the HTML file.

3. **Add Images**:
   - Upload image files corresponding to the entries in the `IMAGE_LABELS` object. Ensure the file names match.

4. **Run the Application**:
   - Open the `index.html` file in a browser, or serve it through a web server.

## Usage

1. Launch the application in a browser.
2. Follow the instructions to select all images matching the displayed category.
3. Submit your selection.
   - If correct, a success message appears.
   - If incorrect, you are prompted to try again with a new CAPTCHA.

## Customization

### Modify Images and Categories

To change the images or categories:

1. Edit the `IMAGE_LABELS` object in the JavaScript code:
   ```javascript
   const IMAGE_LABELS = {
       "newimage1.jpg": "newcategory1",
       "newimage2.jpg": "newcategory2",
       ...
   };
   ```
2. Add corresponding images to the `images` directory.

### Adjust Grid Size or Layout

Modify the grid in the CSS file:
```css
.captcha-grid {
    grid-template-columns: repeat(4, 150px); /* Adjust columns */
    gap: 15px; /* Adjust spacing */
}
```

## Dependencies

This project has no external dependencies and uses plain HTML, CSS, and JavaScript.

## Future Enhancements

- **Backend Integration**: Serve images and categories dynamically via an API.
- **Accessibility**: Add alt text for images and support keyboard navigation.
- **Multi-Category Challenges**: Require users to select images from multiple categories.
- **Mobile Optimization**: Enhance layout and interaction for smaller screens.

## License

This project is open-source and available under the [MIT License](LICENSE).

---

Enjoy using the Category-Based CAPTCHA project! Contributions and feedback are welcome.
