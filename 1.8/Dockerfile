# Start from the alpine image that is smaller but no fancy tools
FROM ubuntu:18.04

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the hello.sh file from this location to /usr/src/app/ creating /usr/src/app/hello.sh
COPY commands.sh .

# Alternatively, if we skipped chmod earlier, we can add execution permissions during the build.
RUN chmod +x commands.sh

# Alternatively, if we skipped chmod earlier, we can add execution permissions during the build.
RUN apt-get update

# Alternatively, if we skipped chmod earlier, we can add execution permissions during the build.
RUN apt-get install curl -y

# When running docker run the command will be ./hello.sh
CMD ./commands.sh
