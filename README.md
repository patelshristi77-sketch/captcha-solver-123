## Simple Captcha Solver

This is a simple web-based Captcha solver interface. It allows users to load a captcha image (either by URL or using a default local image) and then enter the characters they see in the image.

### Features

*   **Load Image by URL**: Users can input an image URL to load any captcha image.
*   **Default Image**: If no URL is provided, a default `sample.png` image is used.
*   **Captcha Input**: A text field to enter the captcha solution.
*   **Verification**: For the `sample.png` image, it checks against a hardcoded correct answer.
*   **Dynamic Feedback**: Provides instant feedback on whether the captcha was solved correctly or if it's an unverified type.
*   **Responsive Design**: Built with Tailwind CSS for a mobile-friendly layout.

### How to Use

1.  **Clone the repository** (or save the `index.html` and `sample.png` files).
2.  **Open `index.html`** in your web browser.
3.  **Load Captcha Image**:
    *   Enter an image URL in the "Image URL" field and click "Load Image".
    *   Alternatively, the `sample.png` will be displayed by default.
4.  **Enter Captcha**:
    *   Type the characters you see in the captcha image into the "Enter Captcha" field.
5.  **Solve**:
    *   Click the "Solve Captcha" button. The application will tell you if your answer is correct (for `sample.png`) or if it cannot verify the captcha.

### Development Notes

*   The correct answer for `sample.png` is hardcoded in the JavaScript (`correctCaptcha = "ADuR3"`).
*   Loading an image from a URL dynamically changes the `src` attribute of the `<img>` tag.
*   The application uses `DOMContentLoaded` to load an initial image if a `url` query parameter is present in the URL.

### Technologies Used

*   HTML5
*   Tailwind CSS (via CDN)
*   JavaScript (Vanilla)
