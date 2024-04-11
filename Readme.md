# Flask Code Challenge - Pizza Restaurants

This is a Flask application for the Pizza Restaurants code challenge.

## Setup and Installation

1. Set the application environment variables:

```bash
export FLASK_APP=app.py
export FLASK_RUN_PORT=5555

Initialize the database:
flask db init

This will create a new directory migrations with several files. You may need to edit the alembic.ini file with your specific configuration/connection/logging settings.

Run the migrations:
flask db migrate -m 'Initial migration!'

This command detects the tables ‘pizzas’, ‘restaurants’, and ‘restaurant_pizzas’ and generates a migration script.

Apply the migrations:
flask db upgrade head

This command runs the upgrade and applies the migration to the database.

Running the Application
To run the application, use the following command:

flask run

This will start the Flask development server on the port specified in the FLASK_RUN_PORT environment variable.