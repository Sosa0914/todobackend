FROM sosa0914/todobackend-base:latest
MAINTAINER Hidenori Yoshizumi <hyoshizumi@hotmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse
