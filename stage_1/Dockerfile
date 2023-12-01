FROM python:3.8-slim

WORKDIR /app

# Copy the requirements file into the container
COPY requirements.txt .

# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt

# Copy the current directory contents into the container at /app
COPY . /app

# Make port 80 available to the world outside this container
EXPOSE 80

# Define environment variable
ENV APP_NAME "Docker_Workshop_Stage_1"

# Run app.py when the container launches
CMD ["python", "app.py"]

# command to build
# docker build -t workshop_stage_1 .

# To connect to the flask app running in the container
# docker run -p 80:80 workshop_stage_1

# type this in the url to see the page
# http://localhost:80/