FROM python:3.8-alpine

WORKDIR /app
COPY . /app

# Install TensorFlow 1.0.0 from the specified wheel file
RUN pip install --no-cache-dir --upgrade https://storage.googleapis.com/tensorflow/mac/cpu/tensorflow-1.0.0-py3-none-any.whl


# Upgrade pip and install dependencies
# RUN apk add --no-cache build-base && pip install --upgrade pip && pip install -r requirements.txt && apk del build-base

# Upgrade pip and install any other needed dependencies specified in requirements.txt
RUN pip install --upgrade pip && pip install -r requirements.txt


CMD python app.py