# Medical Text API

## Overview

The Medical Text API is a tool designed to optimize medical text for different audiences. Whether you're addressing the general public or a specialized audience, this API can tailor the language and complexity of medical information to suit the intended readers. The API is currently in a free beta version, but future plans include monetization.

## Features

- **Text Optimization:** Tailor medical text to different audiences (e.g., general public, medical professionals).
- **Easy Integration:** Simple API endpoints that can be easily integrated into any application.
- **Scalable:** Built with scalability in mind to support a growing number of users.

## Getting Started

### Prerequisites

- Node.js (version 14.x or higher)
- npm (version 6.x or higher)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/nickjlamb/medical-text-api.git
   cd medical-text-api
   ```

2. Install the dependencies:
   ```bash
   npm install
   ```

3. Start the API:
   ```bash
   node index.js
   ```

### Usage

Once the API is running, you can use the following endpoints:

- **Optimize Text Endpoint**
  - **URL:** `/optimize-text`
  - **Method:** `POST`
  - **Description:** Optimizes medical text for a specified audience.
  - **Request Parameters:**
    - `text` (string): The medical text to be optimized.
    - `audience` (string): The target audience (e.g., `general-public`, `medical-professionals`).
  - **Example Request:**
    ```bash
    curl -X POST http://localhost:3000/optimize-text \
    -H "Content-Type: application/json" \
    -d '{
        "text": "This is a sample medical text.",
        "audience": "general-public"
    }'
    ```

  - **Example Response:**
    ```json
    {
      "optimizedText": "Optimized text for general-public: This is a sample medical text."
    }
    ```

- **Status Endpoint**
  - **URL:** `/status`
  - **Method:** `GET`
  - **Description:** Checks the status of the API.
  - **Example Request:**
    ```bash
    curl http://localhost:3000/status
    ```
  - **Example Response:**
    ```json
    {
      "status": "API is running"
    }
    ```

## Contributing

Contributions are welcome! If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are reviewed and merged as appropriate.

## License

This project is licensed under the [MIT License](LICENSE). See the LICENSE file for more details.

## Future Plans

- **Monetization:** The API is currently free to use during the beta phase, but plans are in place to introduce a paid model in the future.
- **New Features:** We are planning to add more customization options and support for additional languages.

## Contact

If you have any questions or need further assistance, feel free to contact the project maintainer:

- **Name:** Nick Lamb
- **Email:** nick@medcopywriter.com

---

This README should now be ready to include in your GitHub repository.
