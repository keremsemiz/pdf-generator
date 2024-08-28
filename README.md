# PDF Generator API

This is a FastAPI-based API for generating PDFs. You can send a title and text, and the API will generate a PDF document containing that text.

## Features

- **Generate PDF**: Create a PDF with a given title and text content.

## Installation

### Using Poetry

1. Clone the repository:
    ```bash
    git clone https://github.com/keremsemiz/pdf-generator.git
    cd pdf-generator-api
    ```

2. Install dependencies:
    ```bash
    poetry install
    ```

3. Run the application:
    ```bash
    poetry run uvicorn pdf_generator_api.main:app --reload
    ```

### Using Pip

1. Clone the repository:
    ```bash
    git clone https://github.com/keremsemiz/pdf-generator.git
    cd pdf-generator-api
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the application:
    ```bash
    uvicorn pdf_generator_api.main:app --reload
    ```

## Usage

After starting the application, you can interact with the API at `http://127.0.0.1:8000`.

### Endpoint

- **POST /generate-pdf/**: Generate a PDF from the provided title and text.
  - Request Body: 
    ```json
    {
      "title": "Sample PDF",
      "text": "This is the content of the PDF."
    }
    ```
  - Response: A PDF file with the provided content.

You can also explore the API documentation by visiting `http://127.0.0.1:8000/docs` in your browser.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
