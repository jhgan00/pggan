FROM tensorflow/tensorflow:1.6.0-py3

# Copies the training code inside the container
COPY *.py /opt/ml/code/
COPY metrics /opt/ml/code/metrics
COPY requirements-pip.txt /opt/ml/code/requirements-pip.txt

RUN pip install --upgrade pip
RUN pip install sagemaker-containers
RUN pip install -r /opt/ml/code/requirements-pip.txt