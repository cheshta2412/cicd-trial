# Use a base image, e.g., Python 3.8
FROM python:3.8-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements.txt file from the prod directory into the container
COPY prod/requirements.txt .

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code from the prod directory into the container
COPY prod/ .

# Define the command to run the application
CMD ["python", "app.py"]


# # Use an official Python runtime as a parent image
# FROM python:3.8-slim

# # Set the working directory in the container
# WORKDIR /app

# # Copy the current directory contents into the container at /app
# COPY . /app

# # Install any needed packages specified in requirements.txt
# RUN pip install --no-cache-dir -r requirements.txt

# # Make port 8080 available to the world outside this container
# EXPOSE 8080

# # Define environment variable
# ENV FLASK_ENV=production

# # Run app.py when the container launches
# CMD ["python", "app.py"]
