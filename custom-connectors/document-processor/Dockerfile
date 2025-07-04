FROM opencti/connector-import-document:6.7.2

# Install additional dependencies for document processing (Alpine Linux)
RUN apk update && apk add --no-cache \
    poppler-utils \
    tesseract-ocr \
    tesseract-ocr-data-eng \
    file \
    py3-magic

# Create necessary directories
RUN mkdir -p /tmp/import-document && \
    chmod 777 /tmp/import-document
