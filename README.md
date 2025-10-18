# AI-Powered CAPTCHA Solver

## Overview

This project provides an intelligent CAPTCHA solver designed to automatically decipher and solve image-based CAPTCHAs. It can process CAPTCHA images provided via a URL parameter or a default attached sample image.

## Features

*   **URL-based Image Input:** Solves CAPTCHAs from publicly accessible URLs specified with the `?url=` query parameter.
*   **Default Sample Image:** Includes a fallback mechanism to solve a pre-attached sample CAPTCHA image if no URL is provided.
*   **Image Processing Pipeline:** Employs advanced image processing techniques for noise reduction and character isolation.
*   **Machine Learning Model:** Utilizes a trained machine learning model for accurate character recognition.
*   **RESTful API:** Exposes a simple API endpoint for easy integration.

## Usage

To use the CAPTCHA solver, send a GET request to the application's endpoint.

**Solving a CAPTCHA from a URL:**

```bash
curl "http://your-app-url.com/?url=https://example.com/path/to/your/captcha.png"
```

**Solving the default sample CAPTCHA:**

```bash
curl "http://your-app-url.com/"
```

The response will be a JSON object containing the solved CAPTCHA text.

## Technical Details

The application is built using Python with Flask for the web framework. Image processing is handled by libraries like OpenCV and Pillow. Character recognition is powered by a Convolutional Neural Network (CNN) trained on a diverse dataset of CAPTCHA images. The model architecture and training process are optimized for speed and accuracy.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.