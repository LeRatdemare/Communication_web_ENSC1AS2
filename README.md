# Communication_web_ENSC1AS2
Cours collaboratif de Communication web pour l'année 2022/2023 au S2 (ENSC).

# Comment ça marche ?

## Utilisation générale

Pour participer à la rédaction du cours en créant le moins de conflits possibles, il faut mettre en place quelques règles :
  - Toutes les pages HTML seront placées dans le dossier html (logique xD), jusqu'à ce que le README change, ça sera 1 page par CM en gros
  - ça serait top que toutes les pages soient reliées au même fichier css, sentez vous libres de le modifier à votre sauce

## Récupérer et exécuter le projet

### Cloner le dépôt
Afin de récupérer le dépôt GitHub ici-présent pour en faire une copie sur votre machine (que l'on appelera donc dépôt local) :
1. J'ouvre un terminal GitBash (ou n'importe quel autre terminal, sur VSCode par exemple)
2. Je me place dans le dossier où je veux mettre mon dépôt en faisant `cd C:/leCheminVersMonDossier`
3. Toujours depuis le terminal je fais `git clone https://github.com/LeRatdemare/Communication_web_ENSC1AS2` (lien récupérable depuis l'onglet *Code* de l'interface GitHub)
    - Je remarque que la commande a créé un nouveau dossier **Communication_web_ENSC1AS2** à l'intérieur du dossier dans lequel je me trouvais. C'est bien ce sous-dossier qu'on appelle "dépôt local" !
    - Pour pouvoir exécuter des commandes Git (ex : `git add ...`, `git branch`, etc...) relatives à ce dépôt je dois d'abord me placer dedans en faisant <code>cd C:/leCheminVersMonDossier/<b>Communication_web_ENSC1AS2</b></code>

### Lancer le site

Pour lancer le site il suffit d'aller dans le dépôt local, dans le dossier **html**, puis sur le cours que vous voulez lancer vous faites "clique droit->Ouvrir avec->Chrome" et c'est bon.
Pas besoin de lancer de terminal ni d'utiliser d'éditeur de code (comme VSCode par exemple) !

## Travailler avec Git/GitHub

1. Je ne travaille JAMAIS sur la branche **main** -> Ne jamais faire <code>git checkout <b>main</b></code>
2. Quand je ne suis pas encore entrain de travailler sur qqch en particulier je me met sur la branche **dev-branch**
    - La 1ère fois faire <code>git checkout -b <b>dev-branch</b></code> pour créer la branche et vous mettre dessus directement
    - Les autres fois faire <code>git checkout <b>dev-branch</b></code> (plus besoin de la recréer)
3. Si je veux commencer à travailler sur une nouvelle fonctionnalité/partie du site je crée une sous branche de **dev-branch**
    1. Je vérifie que je suis bien sur **dev-branch** en faisant `git branch`
    2. Si c'est bon je crée ma branche et je me mets dessus en faisant <code>git checkout -b <b>maNouvelleBranche</b></code>
    3. Enfin, je pousse ma branche sur le dépôt distant (GitHub) en faisant <code>git push origin <b>maNouvelleBranche</b></code> pour que les autres puissent y accéder aussi
4. Lorsque je veux apporter des modifications sur une branche, je commence ***toujours*** par me mettre à jour sur celle-ci :
    1. Je fais <code>git pull origin <b>maNouvelleBranche</b></code>
    2. Je peux aussi me mettre à jour sur les dernières mises à jour générales de temps en temps en faisant <code>git pull origin <b>dev-branch</b></code> en étant sur **maNouvelleBranche**.
5. Pendant que je travaille je peux régulièrement faire des commits :
    1. En étant sur **maNouvelleBranche** je fais `git add fichier1.html` pour chaque fichier que j'ai mis à jour (ici fichier1.html)
    2. Toujours au même endroit je fais <code>git commit -m <em>"Un super message bien descriptif de ce que je viens de faire"</em></code> après avoir ajouté tous les fichiers (étape précédente)
6. Une fois que j'ai fini une session de travail je fais systématiquement un dernier commit puis je partage mon travail sur GitHub
    - Pour ça je fais simplement <code>git push origin <b>maNouvelleBranche</b></code>
7. Si jamais j'ai terminé d'implémenter une fonctionnalité, je n'ai plus besoin d'utiliser la branche donc je fais une pull request :
    1. Je commence par me replacer sur la **dev-branch** en faisant <code>git checkout <b>dev-branch</b></code>
    2. Depuis l'interface GitHub, je suis les étapes pour faire une pull-request et j'attends qu'un modérateur l'accepte
    3. Une fois qu'elle aura été acceptée je pourrais suprimer **maNouvelleBranche** sur mon dépôt locale en faisant <code>git branch -D <b>maNouvelleBranche</b></code>
    4. Je peux quand même commencer à travailler sur un nouvelle branche (étape n°3) en attendant que la pull request soit acceptée
  
