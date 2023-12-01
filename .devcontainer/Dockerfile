FROM jupyter/pyspark-notebook:latest

# Add netcat (nc) to run spark socket streaming examples
USER root
RUN apt update && apt install -y \
    netcat

USER $NB_USER

# any additional packages
RUN conda install pyspark

RUN pip install tensorflow
