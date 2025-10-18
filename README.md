# AI-Powered CAPTCHA Solver

## Overview

This project provides an automated solution for solving image-based CAPTCHAs. It takes a URL pointing to a CAPTCHA image and leverages AI models to accurately identify and return the text content of the CAPTCHA. A default sample image is included for immediate testing.

## Features

*   **URL-based Image Input**: Solves CAPTCHAs from provided image URLs.
*   **Default Sample Image**: Includes a pre-attached sample image for quick demonstration.
*   **AI-driven Recognition**: Utilizes advanced machine learning models for high accuracy.
*   **Text Output**: Returns the solved CAPTCHA text in a clear format.

## Usage

1.  **Clone the repository:**
    ```bash
    git clone <repository_url>
    cd captcha-solver-123
    ```

2.  **Run the solver:**
    *   **With a URL:**
        ```bash
        python main.py --url <image_url>
        ```
        Replace `<image_url>` with the actual URL of the CAPTCHA image.

    *   **Using the default sample image:**
        ```bash
        python main.py
        ```

The solved CAPTCHA text will be printed to the console.

## Technical Details

This application utilizes a Python backend. The core CAPTCHA solving functionality is powered by a pre-trained Optical Character Recognition (OCR) model. The model is responsible for analyzing the image pixels and converting them into readable text. The application handles image fetching from URLs and processes them for the OCR engine.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.