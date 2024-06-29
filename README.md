# Wildlife Blog Website

Welcome to the Wildlife Blog Website repository! This project is a fully-functional web application built using Flask, designed to create and manage a blog dedicated to wildlife content. Here is a brief overview of the main features and components of this project:

## Key Features:
- **User Authentication:** Secure user registration and login functionality using Flask-Login and password hashing with Werkzeug.
- **Post Management:** Logged-in users can create, edit, and delete blog posts. Only authenticated users are allowed to perform these actions.
- **Commenting System:** Users can comment on blog posts. Only logged-in users can submit comments to maintain the quality of discussions.
- **Gravatar Integration:** Gravatar is used to display user avatars in the comment section.
- **Responsive Design:** The website uses Flask-Bootstrap to ensure a responsive and modern design.
- **WYSIWYG Editor:** CKEditor integration for rich text editing of blog posts.
- **Email Notifications:** Contact form submissions are sent directly to the site administrator via email using SMTP.

## Technology Stack:
- **Flask:** The core framework used for developing the web application.
- **SQLAlchemy:** ORM for database interactions.
- **Flask-Login:** Manages user sessions and authentication.
- **Flask-Bootstrap:** Ensures the site is responsive and visually appealing.
- **Flask-CKEditor:** Provides a rich text editor for creating blog posts.
- **Flask-Gravatar:** Integrates Gravatar for user avatars in comments.
- **Environment Variables:** Configuration of sensitive data using environment variables.

## Database:
- **SQLite/PostgreSQL:** Configurable database options, defaulting to SQLite for simplicity but easily adaptable to PostgreSQL.

## Getting Started:
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/wildlife-blog.git
   cd lambda_project/Blog-website
2. **Set Up the Environment:**
   Install the required packages:
   ```bash
   pip install -r requirements.txt
3. **Setiing up Environment Variables:**
   Create a .env file in the root directory and add your configurations.
   ```bash
   MY_EMAIL=your-email@example.com
   MY_PASSWORD=your-email-password
   DB_URI=your-database-uri  # use this if you want to configure database to PostgreSQL
4. **Database Initialization:**
   Run the following commands to set up the database:
   ```bash
   flask db init
   flask db migrate
   flask db upgrade
5. **Running the Application:**
   Start the Flask development server:
   ```bash
   flask run
  Access the website at http://127.0.0.1:5000.
