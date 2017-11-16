FROM asarchami/oscore:latest
MAINTAINER Ali Sarchami

ENV DATAPUSHER_HOME /usr/lib/datapusher

RUN mkdir -p $DATAPUSHER_HOME/src && \
    git clone -b '0.0.13' https://github.com/ckan/datapusher.git \
        $DATAPUSHER_HOME/src/datapusher

WORKDIR $DATAPUSHER_HOME/src/datapusher

RUN pip install -r requirements.txt && \
    pip install -e .

EXPOSE 8800

CMD [ "python", "datapusher/main.py", "deployment/datapusher_settings.py" ]
