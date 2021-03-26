# Currently working with precommit and python and wanted to have a docker based config
# This image is used as a base to run all python checks.
# For now the version is hardcoded to 3.7.10 as that is what is being used on the project.

FROM python:3.7.10-stretch

RUN pip install -U virtualenv
RUN python -m virtualenv /venv
RUN /venv/bin/python -m pip install -U black isort pytype

ENV PATH=/venv/bin:$PATH
