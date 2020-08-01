# Docker
### Créer une image Docker

Faire un Dockerfile pour y mettre des instructions

exemple:

    FROM python:2.7-slim
    WORKDIR /app
    COPY . /app
    RUN pip install -r requirements.txt
    EXPOSE 80
    ENV NOM moi
    CMD ["python", "app.py"]


|Mots clés **Dockerfile**||
|--|--|
|**FROM**|  Image de base  |  
|**WORKDIR**|  Répertoire courant  |  
|**COPY**|  Copie des fichiers dans l'image  |  
|**RUN**|  Exécuter des commandes  (installation de dépendance)  
|**EXPOSE**|  Exposer des ports  |  
|**ENV  NOM**|  Variable d’environnement  |  
|**CMD**|  Commande à exécuter au lancement  |

Pour créer l'image 

    docker build -t *NOM-IMG* .
    
Pour lancer le conteneur :

    docker run -d *NOM-IMG*
