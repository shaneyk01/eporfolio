# Personal Portfolio Website

This project is a modern, responsive personal portfolio website designed to showcase skills, projects, and professional background. The site features a clean, dark-themed aesthetic with interactive elements to provide an engaging user experience. It is built with HTML5, CSS3, and Bootstrap 5.

## How Bootstrap Was Used

This project heavily utilizes the Bootstrap 5 framework to ensure responsiveness and a consistent design across different devices. Key components used include:

*   **Navbar (`navbar`):** For the main site navigation, which is sticky and collapses on smaller screens.
*   **Grid System (`container`, `row`, `col`):** To create flexible and responsive layouts for all pages, especially for project cards and page content.
*   **Cards (`card`):** To display individual projects in a structured and visually appealing format.
*   **Buttons (`btn`):** For calls-to-action, links, and form submissions, with custom styling.
*   **Modal (`modal`):** To display additional information in the "About Me" section without navigating away from the page.
*   **Accordion (`accordion`):** Used on the "About Me" page to organize and present detailed information in a collapsible format.
*   **Form Controls (`form-control`, `form-label`):** To build the contact form with a clean and user-friendly layout.

## JavaScript Functions & Future Integration (`part2.js`)

The `part2.js` file contains a collection of reusable JavaScript functions ready to be integrated into the website to add advanced functionality.

### 1. Dynamic Theme Toggler (`toggleTheme`)
*   **Summary:** This function allows users to switch between a 'dark' and 'light' theme. It saves the user's preference in their browser's local storage, so their chosen theme will be remembered on their next visit.
*   **Future Integration:** To use this, you would first need to add CSS styles for a `.light-mode` class. Then, you could add a toggle switch or button to the navbar that calls the `toggleTheme()` function when clicked.

### 2. Typewriter Effect (`typeWriter`)
*   **Summary:** This function creates a "typing" animation for any text element on the page. It makes text appear one character at a time, which is a great way to draw attention to a headline.
*   **Future Integration:** This could be used on the homepage's main heading. You would select the heading element and call the function with the text you want to animate, like this: `typeWriter(document.querySelector('.hero h1'), 'Welcome to My Portfolio');`

### 3. "Back to Top" Button (`setupBackToTopButton`)
*   **Summary:** This function creates a button that appears only after the user has scrolled down the page. When clicked, it smoothly scrolls the page back to the top. This is very useful for long pages.
*   **Future Integration:** First, add a button element to your HTML (e.g., `<button id="backToTopBtn">Top</button>`) and style it with CSS. Then, call `setupBackToTopButton('backToTopBtn')` when the page loads to make it work.

### 4. Lazy Loading for Images (`enableLazyLoading`)
*   **Summary:** This function improves website performance by only loading images when they are about to enter the screen. This makes the initial page load much faster, especially on pages with many images.
*   **Future Integration:** To implement this, you would add a class (e.g., `class="lazy"`) to all the images you want to lazy load. You would also change their `src` attribute to `data-src`. Finally, you would call `enableLazyLoading('.lazy')` when the page loads.
