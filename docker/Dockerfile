FROM python:3

RUN git clone https://github.com/seadowg/pyxform.git
WORKDIR "/pyxform"
RUN python setup.py develop

WORKDIR "/"
RUN rm -r pyxform

RUN pip install nose==1.0.0
RUN apt-get update && apt-get install -y default-jre
