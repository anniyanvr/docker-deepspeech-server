FROM tensorflow/tensorflow:1.15.2-gpu-py3

RUN pip3 install --upgrade pip

COPY gpu/requirements.txt /tmp
RUN pip3 install --no-cache-dir -r /tmp/requirements.txt

ENTRYPOINT deepspeech-server --config /opt/deepspeech/config.json
