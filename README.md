# Communication_web_ENSC1AS2
Cours collaboratif de Communication web pour l'année 2022/2023 au S2 (ENSC).

# Comment ça marche ?

## Utilisation générale
Pour participer à la rédaction du cours en créant le moins de conflits possibles, il faut mettre en place quelques règles :
    - Toutes les pages HTML seront placées dans le dossier html (logique xD), jusqu'à ce que le README change, ça sera 1 page par CM en gros
    - ça serait top que toutes les pages soient reliées au même fichier css, sentez vous libres de le modifier à votre sauce

## Travailler avec Git/GitHub

1. Je ne travaille JAMAIS sur la branche **main** -> Ne jamais faire "git checkout **main**"
2. Quand je ne suis pas encore entrain de travailler sur qqch en particulier je me met sur la branche **dev-branch**
    - La 1ère fois faire "git checkout -b **dev-branch**" pour créer la branche et vous mettre dessus directement
    - Les autres fois faire "git checkout **dev-branch**" (plus besoin de la recréer)
3. Si je veux commencer à travailler sur une nouvelle fonctionnalité/partie du site je crée une sous branche de **dev-branch**
    1. Je vérifie que je suis bien sur **dev-branch** en faisant "git branch"
    2. Si c'est bon je crée ma branche et je me mets dessus en faisant "git checkout -b **maNouvelleBranche**"
4. Lorsque je veux apporter des modifications sur une branche, je commence ***toujours*** par me mettre à jour sur celle-ci :
    1. Je fais "git pull origin **maNouvelleBranche**"
    2. Je peux aussi me mettre à jour sur les dernières mises à jour générales de temps en temps en faisant "git pull origin **dev-branch**" en étant sur **maNouvelleBranche**.
5. Pendant que je travaille je peux régulièrement faire des commits :
    1. En étant sur **maNouvelleBranche** je fais "git add fichier1.html" pour chaque fichier que j'ai mis à jour (ici fichier1.html)
    2. Toujours au même endroit je fais "git commit -m *"Un super message bien descriptif de ce que je viens de faire"*" après avoir ajouté tous les fichiers (étape 1)
6. Une fois que j'ai fini une session de travail je fais systématiquement un dernier commit puis je partage mon travail sur GitHub
    - Pour ça je fais simplement "git push origin **maNouvelleBranche**"
7. Si jamais j'ai terminé d'implémenter une fonctionnalité, je n'ai plus besoin d'utiliser la branche donc je fais une pull request :
    1. Je commence par me replacer sur la **dev-branch** en faisant "git checkout **dev-branch**"
    2. Depuis l'interface GitHub, je suis les étapes pour faire une pull-request et j'attends qu'un modérateur l'accepte
    3. Une fois qu'elle aura été acceptée je pourrais suprimer **maNouvelleBranche** sur mon dépôt locale en faisant "git branch -D **maNouvelleBranche**"
    4. Je peux quand même commencer à travailler sur un nouvelle branche (étape n°3) en attendant que la pull request soit acceptée
  
