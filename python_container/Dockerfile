FROM python:3.9-alpine

WORKDIR /usr/src/app

COPY requirements.yml . 
#RUN pip install --upgrade pip; pip install -r requirements.yml ; conda install python
#RUN pip install --upgrade pip; pip install -r requirements.yml ; apt-get install python3-pandas 
RUN pip install --upgrade pip; pip install -r requirements.yml 

