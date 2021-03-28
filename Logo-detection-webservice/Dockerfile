# Create the base image
FROM python:3.7-slim

RUN apt-get install ca-certificates

# Copy local folder into the container
#COPY ./* /app/ - to copy all files into root level
COPY ./ /app/

# Change the working directory
WORKDIR /app/

# Install Dependency
RUN pip install -r requirements.txt


# Set "python" as the entry point
ENTRYPOINT ["python"]

# Set the command as the script name
CMD ["app.py"]