### Examen Clusteurisation 
Auteur : DEGEZ Gabriel
Date : vendredi 6 mai 2022
Lieu : CFA Insta

1 - J'ai crée le fichier *deployment_DEGEZ.yml* qui fait le déploiement de pod de redis vers le cloud. Puis j'ai fait kubectl *create -f deployment_DEGEZ.yml* et *kubectl get pods* pour vérifier.

2 - J'ai crée le fichier *deployment_server_DEGEZ.yml* qui fait la même chose vers le service nodejs. Puis j'ai fait *kubectl create -f deployment_server_DEGEZ.yml* et *kubectl get pods* pour vérifier.

3 - J'ai crée le fichier *service_DEGEZ.yml* qui lancer les services.

4 - J'ai récupére l'adresse IP en faisant kubectl get services et je l'ai mise dans le fichier *deployment_server_DEGEZ.yml*. J'ai fait *kubectl logs <pod-id>* pour vérifier que tout fonctionne.

5 - Dans *deployment_DEGEZ.yml*, j'ai modifié replicas (le nombre de pods) et ca fonctionne toujours.