FROM python:3.9-slim

RUN pip install -U pip
RUN pip install pipenv


WORKDIR '/Users/agvg/Documents/DS/MLOPS/MLOPS/Class 4'

COPY [ "Pipfile", "Pipfile.lock", "./" ]

RUN pipenv install --system --deploy

COPY [ "Homework4.py", "model.bin", "./" ]

ENTRYPOINT ["python3.9","./Homework4.py"]