FROM python:3.11

LABEL maintainer ArquiteturaDeSolucoes
LABEL name=hello-python-pdec version=1.0
RUN mkdir /app
WORKDIR /app
ADD . /app/
RUN pip install -r requirements.txt

ARG PORT_BUILD=5000
ENV PORT=$PORT_BUILD
EXPOSE $PORT_BUILD
CMD ["python", "/app/main.py"]