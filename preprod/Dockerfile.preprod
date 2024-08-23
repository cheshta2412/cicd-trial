# Use the official Python image from the Docker Hub
FROM python:3.8-slim

# Set the working directory
WORKDIR /app

# Copy the requirements.txt file into the container
COPY requirements.txt .

# Install the Python dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code into the container
COPY . .

# Expose the port the app runs on
EXPOSE 8080

# Set the environment variable
ENV FLASK_APP=app.py

# Run the application
CMD ["flask", "run", "--host=0.0.0.0", "--port=8080"]



# # Use the official Python image from the Docker Hub
# FROM python:3.8-slim

# # Set the working directory
# WORKDIR /app

# # Copy the requirements file into the container
# COPY requirements.txt .

# # Install dependencies
# RUN pip install --no-cache-dir -r requirements.txt

# # Copy the application code into the container
# COPY app.py .

# # Expose the port the app runs on
# EXPOSE 8080

# # Command to run the application
# CMD ["python", "app.py"]


# # Use a Python image from Docker Hub
# FROM python:3.8-slim

# # Set the working directory
# WORKDIR /app

# # Copy the requirements file into the container
# COPY requirements.txt .

# # Install dependencies
# RUN pip install --no-cache-dir -r requirements.txt

# # Copy the application code into the container
# COPY app.py .

# # Specify the command to run the application
# CMD ["python", "app.py"]
