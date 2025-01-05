FROM python:3.13

EXPOSE 5000

WORKDIR /app

COPY requirements.txt /app
RUN pip install -r requirements.txt

# COPY app.py /app
# CMD python app.py

# Copy the 'app' directory contents (app.py and other files) into the container
COPY . /app

# Set the FLASK_APP environment variable to point to the app instance
# This will look for the 'app' module inside the 'app' directory
# ENV FLASK_APP=app.app  

# Set the default command to run the Flask app with the correct host and port
CMD ["flask", "run", "--host", "0.0.0.0"]