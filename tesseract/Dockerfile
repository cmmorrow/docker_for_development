FROM ubuntu:bionic
LABEL maintainer="cmmorrow@gmail.com"
RUN apt-get update && apt install -y tesseract-ocr libtesseract-dev
WORKDIR /tesseract
ENTRYPOINT ["tesseract"]

