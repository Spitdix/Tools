# Docker
Créer une image Docker
Faire un Dockerfile pour y mettre des instructions
exemple:

    FROM python:2.7-slim
    WORKDIR /app
    COPY . /app
    RUN pip install -r requirements.txt
    EXPOSE 80
    ENV NOM moi
    CMD ["python", "app.py"]

**FROM** 
**WORKDIR** 
**COPY** 
**RUN**
**EXPOSE** 
**ENV NOM**
**CMD**
