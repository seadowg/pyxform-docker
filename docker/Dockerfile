FROM python:3

RUN git clone https://github.com/XLSForm/pyxform.git
WORKDIR "/pyxform"
RUN git checkout 66c0d5b9ad4a34bce47fe52a60e4366c19ee457c
RUN pip install -r dev_requirements.pip

WORKDIR "/"
RUN rm -r pyxform

RUN apt-get update && apt-get install -y default-jre
