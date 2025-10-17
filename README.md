# Simple Captcha Solver

This is a basic, single-file web application designed to demonstrate a client-side interface for solving captchas. It allows users to load a captcha image, input their solution, and check if it's correct.

## Features

-   **Image Loading:** Load captcha images from a specified URL or default to the included `sample.png`.
-   **URL Parameter Support:** Automatically loads an image if a `?url=` parameter is provided in the browser's address bar.
-   **User Input:** Provides an input field for users to type their captcha solution.
-   **Solution Verification:** For the default `sample.png` image, it verifies the user's input against the known correct answer ("ADuR3"). For other images loaded via URL, it indicates that verification is not supported client-side without a backend.
-   **Responsive Design:** Built with Tailwind CSS for a mobile-friendly and responsive user interface.

## How to Run

1.  **Save the files:** Save `index.html`, `README.md`, and `sample.png` in the same directory.
2.  **Open `index.html`:** Open `index.html` in your web browser.

### Loading Custom Captchas

You can load a custom captcha image in two ways:

1.  **Using the Input Field:** Type the URL of your captcha image into the "Image URL" field and click "Load Image".
2.  **Using a URL Parameter:** Append `?url=YOUR_IMAGE_URL` to the `index.html` URL in your browser. For example:
    `file:///path/to/your/index.html?url=https://example.com/some-other-captcha.png`

## Technologies Used

-   **HTML5:** Structure of the web page.
-   **Tailwind CSS:** For styling and responsive design.
-   **JavaScript:** For interactive elements, image loading logic, and client-side captcha verification (for `sample.png`).