

```markdown
# Preview
![Image Uploader Screenshot](/p2.jpeg)

# Flask Authentication System

This is a simple authentication system built using Flask. It allows users to register, log in, and view a personalized dashboard displaying their username.

## Features

- User Registration
- User Login
- Password Hashing with bcrypt
- Dashboard displaying the logged-in user's name

## Requirements

To install the necessary dependencies, make sure you have `pip` installed and run the following command:

```sh
pip install -r requirements.txt
```

### requirements.txt

```
Flask==2.0.3
Flask-SQLAlchemy==2.5.1
bcrypt==3.2.0
```

## Getting Started

Follow these steps to set up and run the project locally.

### 1. Clone the Repository

```sh
git clone https://github.com/yourusername/flask-authentication-system.git
cd flask-authentication-system
```

### 2. Set Up the Environment

Create a virtual environment to manage dependencies.

```sh
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### 3. Install Dependencies

```sh
pip install -r requirements.txt
```

### 4. Configure the Application

Create a `.env` file to store your configuration variables. Add the following lines to your `.env` file:

```
SECRET_KEY=your_secret_key
SQLALCHEMY_DATABASE_URI=sqlite:///site.db
```

Replace `your_secret_key` with a strong, random string.

### 5. Initialize the Database

Run the following commands to create the database and the necessary tables:

```sh
flask db init
flask db migrate -m "Initial migration."
flask db upgrade
```

### 6. Run the Application

Start the Flask application:

```sh
flask run
```

Your application will be available at `http://127.0.0.1:5000/`.

## Usage

### Registration

Navigate to `http://127.0.0.1:5000/register` to create a new account.

### Login

Navigate to `http://127.0.0.1:5000/login` to log into your account.

### Dashboard

After logging in, you will be redirected to the dashboard at `http://127.0.0.1:5000/dashboard`, where you can see your username displayed.

## Contributing

Contributions are welcome! Please create a pull request or open an issue to discuss any changes.

## License

This project is licensed under the MIT License.
```

You can copy this code into a file named `README.md` in your project repository.