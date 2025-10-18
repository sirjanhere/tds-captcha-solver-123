# AI-Powered CAPTCHA Solver

## Overview

This project provides a web application capable of solving CAPTCHAs from provided image URLs or a default sample image. It leverages AI models to interpret and decode the distorted text within CAPTCHA images, making them programmatically accessible.

## Features

*   **URL-based CAPTCHA Solving:** Accepts a `?url=` query parameter to specify the CAPTCHA image source.
*   **Default Sample Image:** Includes a fallback mechanism to solve a pre-attached sample CAPTCHA image if no URL is provided.
*   **AI-driven Recognition:** Utilizes advanced machine learning models for accurate text extraction from distorted CAPTCHAs.
*   **Web Interface:** Provides a simple web interface for easy interaction and testing.

## Usage

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/captcha-solver-123.git
    cd captcha-solver-123
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the application:**
    ```bash
    python app.py
    ```
4.  **Access the web interface:** Open your browser and navigate to `http://127.0.0.1:5000/`.
5.  **Solve a CAPTCHA:**
    *   To solve the default sample CAPTCHA, simply visit the root URL.
    *   To solve a CAPTCHA from a specific URL, append `?url=YOUR_IMAGE_URL` to the root URL. For example: `http://127.0.0.1:5000/?url=https://example.com/path/to/your/captcha.png`

## Technical Details

The application is built using Flask as the web framework. It utilizes pre-trained AI models (e.g., for Optical Character Recognition - OCR) to analyze the image and extract the text. Image processing techniques are applied to enhance readability before feeding to the OCR engine.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.