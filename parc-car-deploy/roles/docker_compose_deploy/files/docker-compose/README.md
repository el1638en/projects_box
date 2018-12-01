## Docker

1.Création de l'image 

  Pour créer une image locale pour la bdd : 
  
```shell
cd postgresql 
docker image build -t parc-car-postgres:latest .                              
```
  On peut vérifier la présence de l'image dans le registry local :
  
```shell
docker image ls -a
REPOSITORY                                      TAG                 IMAGE ID            CREATED             SIZE
parc-car-postgres                             latest              f3ab9569f0a2        4 seconds ago       313MB
```

2.Démarrer la base de données

  ```shell
  cd docker-dev-env
  docker-compose up -d
  ```
