# Image Upload Web App

A simple Flask web application that allows authenticated users to upload, view, and delete image files.

---

## Features

- Upload images (`png`, `jpg`, `jpeg`, `gif`)
- List all uploaded images
- Delete uploaded images
- IP-based access restriction (only allows requests from a specific VPN IP)
- Simple UI for file management

---

## Requirements

- Python 3.7+
- Flask

---

## Setup & Installation

1. Clone the repository:
	git clone https://github.com/Kashikikato/Web-App-with-Image-Upload.git
	cd Web-App-with-Image-Upload

2. Create and activate a virtual environment (optional but recommended):
	
 		python3 -m venv venv

 		source venv/bin/activate  # Linux/macOS

 		venv\Scripts\activate     # Windows

4. Install dependencies:
	pip install flask

5. Create the uploads folder:
	mkdir uploads

6. Run the app:
	flask run

7. Open you browser at http://127.0.0.1:5000

## Configuration

- Allowed file types: `.png`, `.jpg`, `.jpeg`, `.gif`
- IP-based access restriction: 
  - The app only allows requests from a specific IP address (default is `20.218.226.24`)
  - You can change this IP in the `restrict_ip` function inside `app.py` to match your VPN or desired whitelist

---

## Usage

- Upload images directly on the homepage via the upload form
- View the list of uploaded images below the form
- Delete any uploaded image using the provided delete button

---

## Notes

- Access control is based solely on IP filtering; no user authentication is implemented
- Designed for small-scale or internal use, ideally behind a VPN
- Make sure the `uploads` directory exists and is writable by the app
- For production, consider adding authentication and HTTPS for security

---

## Author

Arian Behrami
