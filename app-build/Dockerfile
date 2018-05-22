FROM python:3.6
RUN apt-get -qq update

ENV PATH /opt/conda/bin:$PATH

ENV PATH /opt/conda/bin:$PATH
RUN mkdir /code
WORKDIR /code

ADD requirements.yml /code/
RUN conda env create -f /code/requirements.yml

RUN apt-get update

COPY entrypoint.sh /usr/local/bin/

RUN chmod u+x /usr/local/bin/entrypoint.sh
EXPOSE 5000
ENTRYPOINT ["entrypoint.sh"]




