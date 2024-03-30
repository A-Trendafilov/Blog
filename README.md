# Blog Project

## Prerequisites

Before running the project, ensure you have the following installed:

- Python 3.x
- Flask
- Flask-Bootstrap5
- Flask-SQLAlchemy
- Flask-WTF
- Flask-CKEditor
- SQLAlchemy
- dotenv

You can install the dependencies using pip:

```bash
pip install Flask Flask-Bootstrap5 Flask-SQLAlchemy Flask-WTF Flask-CKEditor SQLAlchemy python-dotenv
```

### Setup

- Clone this repository to your local machine:

```bash
git clone https://github.com/your_username/blog_project.git
```

- Navigate to the project directory:

```bash
cd blog_project
```

- Create a virtual environment:

```bash
python -m venv venv
```

- Activate the virtual environment:
    - On Windows:
      ```bash
      venv\Scripts\activate
      ``` 
    - On macOS and Linux:
      ```bash
      source venv/bin/activate
      ```

- Create a .env file in the project directory and set the following variables:

```makefile
SECRET_KEY=your_secret_key
EMAIL=your_email
PASSWORD=your_email_password
```

Replace your_secret_key, your_email, and your_email_password with your preferred values. Make sure to use a secure and
strong secret key.

- Initialize the SQLite database by running:

```bash
python
```

Then, inside the Python shell:

```python
from app import db

db.create_all()
exit()
```

### Running the Application

To start the Flask server, run:

```bash
python app.py
```

The application will be accessible at http://localhost:5003 in your web browser.

## Usage

### Creating a New Post

- Navigate to the homepage.
- Click on "New Post".
- Fill in the required fields: title, subtitle, author, blog image URL, and content.
- Click on "Submit Post" to create the post.

### Editing a Post

- Navigate to the post you want to edit.
- Click on the "Edit" button.
- Modify the content as needed.
- Click on "Submit Post" to save the changes.

### Deleting a Post

- Navigate to the post you want to delete.
- Click on the "Delete" button.
- Contact Form
- Navigate to the "Contact" page.
- Fill in your name, email, phone (optional), and message.
- Click on "Send Message" to submit the contact form.

### About

- The "About" page provides brief information about the blog project.

### Additional Notes

- This project utilizes Flask for its backend framework.
- Bootstrap5 is used for styling.
- Flask-SQLAlchemy manages the database interactions.
- Flask-WTF is used for form handling.
- Flask-CKEditor is integrated for a rich text editor.
- Contact form functionality is implemented using Flask-Mail.
- Ensure you replace the email and password in the .env file with valid credentials for the contact form to work
  properly.

