ARG BUILD_FROM
FROM $BUILD_FROM
RUN apk add --no-cache python3 py3-pip
#RUN pip3 install smbus2
RUN apt-get --no-cache-dir install build-essential libi2c-dev i2c-tools python-dev libffi-dev
COPY test.py /
COPY run.sh /
RUN chmod a+x /run.sh
CMD [ "/run.sh" ]