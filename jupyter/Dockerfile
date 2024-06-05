# Use an official Python runtime as a parent image
FROM python:3.8
# Optional: Install additional libraries if needed
RUN pip install pandas numpy matplotlib

# Set the working directory to /app
WORKDIR /app


# Install Jupyter Notebook
RUN pip install jupyter

# Make port 8888 available to the world outside this container
EXPOSE 8888

# Define environment variable
ENV NAME World

# Run Jupyter Notebook when the container launches
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
