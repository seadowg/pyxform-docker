FROM python:3

RUN git clone https://github.com/seadowg/pyxform.git
WORKDIR "/pyxform"
RUN python setup.py develop
RUN pip install -r requirements.pip

WORKDIR "/"
RUN rm -r pyxform

RUN apt-get update && apt-get install -y default-jre
