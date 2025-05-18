# COMPLAINT SYSTEM FOR COLLEGE STUDENTS

This project is a web-app based project for accepting complaint from students descriptions using python flask framework and the Azure.

## Features

* **USER-FRIENDLY:**  Users can describe everything in plain English.
* **Solidity Code Generation:** The application uses the Azure services to keep web-app updated based on the as per go rule!  
* **Error Handling:** Basic error handling for invalid requests and spam protection

## Getting Started

### Prerequisites

* flask
* requests
* `requests` library (install with `pip install requests`)
* python-dotenv.
* azure-storage-blob.
* gunicorn

### Installation

1. Clone the repository:
   ```bash
   git clone <repository_url>
   ```
2. Create a virtual environment:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # Activate the virtual environment (adjust for your OS)
    ```

3.  Install dependencies from `requirements.txt`
  ```bash
   pip install -r requirements.txt
   ```

4. Run the development server:
   ```bash
   python manage.py runserver
   ```

## API Usage

**Endpoint:** `/api/generate`
**Method:** `POST`
**Request Body (JSON):**

```json
{
  "description": "Create a complaint that allows users tosolve their problem." 
}
```

**Response (JSON):**

```json
{
  "success": true,
  "message": "complaint generated successfully",
  "generated_code": "complaint raised ..." 
}
```

## Future Improvements

* **Comprehensive Error Handling:**  More robust error handling for various scenarios.
* **Security Enhancements:** Implement proper protection.
* **Code Validation:** Verify the code before returning it to the user.
* **Sandboxing:** Run the code generation and potentially in a sandboxed environment for enhanced security.
* **Frontend Integration:** Develop a user interface for easier interaction with the API.



## Contributing


Contributions are welcome! Please open an issue or submit a pull request.

## License



This project is licensed under the [MIT License](LICENSE).
