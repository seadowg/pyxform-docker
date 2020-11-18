FROM python:3

RUN git clone https://github.com/XLSForm/pyxform.git
WORKDIR "/pyxform"
RUN git checkout 85582ef0f65c07e0062835add92821787c5c8d44
RUN python setup.py develop
RUN pip install -r requirements.pip

WORKDIR "/"
RUN rm -r pyxform

RUN apt-get update && apt-get install -y default-jre
