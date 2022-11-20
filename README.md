# COB-99, l'ordinateur rebranché
COB-99 est un simulateur en COBOL de l'architecture d'ordinateur M99 développée plus amplement [ici](https://github.com/InfoSansOrdi/M999).

Merci à l'équipe d'InfoSansOrdi !

---

## Utilisation
### Paramétrage
L'initialisation du compteur ordinal peut être renseignée et pour l'exécution celle-ci est paramétrable en mode pas-à-pas, c'est-à-dire que l'exécution attend une entrée utilisateur avant d'incrémenter le compteur ordinal.

Attention il y a un fichier externe primordial, le programme nécessite une ROM pour accueillir les instructions à appeler. Par défaut le fichier est `rom.m99` (simple fichier txt).
### Exécution
L'exécution se fait grâce à GNUCOBOL : `cobc -free -x -o m99 m99.cob`, puis `./m99`.

Si vous désirez modifier l'exécution, ouvrez le fichier `rom.99`. Pour modifier veuillez respecter le format `999 999 999...` sur une ligne.
### Prérequis
cobc 3.1.2.0
