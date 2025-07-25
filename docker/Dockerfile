FROM python:3.13.2-alpine

# Install Git (required for pbr versioning)
RUN apk add --no-cache git

# Copy the source code into the container
COPY . /bandit

# Set the working directory
WORKDIR /bandit

# Install Bandit from the source code using pip
RUN pip install .

# Define entrypoint and default command
ENTRYPOINT ["bandit"]
