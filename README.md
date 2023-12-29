
# Spotify popularity prediction

Ce projet entre dans le cadre du cours de 2ème année de l'ENSAE, python pour le cours Python pour la Data Science. Il a pour but la prédiction de la popularité d'une musique en se basant sur ses caractéristiques audio.

La popularité d'une musique étant déjà calculé par spotify, nous utiliserons l'API spotify pour l'extraire. C'est une valeur comprise entre 0 et 100. La popularité est calculée par un algorithme et est principalement basée sur le nombre total de lectures que la musique a eu et sur la récence de ces lectures.








## Explication des variables du Dataset

Voici les descriptions des différentes variables que nous utilisons dans notre projet :


1-  **Key :**
   - La tonalité de la musique. Des entiers correspondant à des notes. Par exemple, 0 = C (Do), 1 = C♯/D♭, 2 = D(Ré), et ainsi de suite. Si aucune tonalité n'a été détectée, la valeur est -1.

Valeurs prises :entiers entre -1 - 11. 

2-  **Mode :**
   - Le mode indique la modalité (majeure ou mineure) d'une musique, c'est-à-dire le type d'échelle à partir duquel le contenu mélodique est dérivé. Le mode majeur est représenté par 1 et le mode mineur par 0.

Valeurs prises : 0 ou 1.

3-  **Time_signature (Signature temporelle) :**
   - C'est une estimation de la signature temporelle. La signature temporelle est une convention de notation qui permet de spécifier le nombre de beats dans chaque période (ou mesure).
Valeurs prises entières entre 3 - 7

4- **acousticness (Acousticité) :**
   - Une mesure de 0.0 à 1.0 indiquant si la musique est acoustique. 1.0 représente une forte probabilité que la piste soit acoustique.

5- **danceability (Dansabilité) :**
   - La dansabilité décrit à quel point une musique est adaptée à la danse en fonction d'une combinaison d'éléments musicaux tels que le tempo, la stabilité du rythme, la force du battement, et la régularité globale. Une valeur de 0.0 est la moins dansable et 1.0 est la plus dansable.
   Varibale float entre 0 et 1

6- **energy (Énergie) :**
   - Une mesure de 0.0 à 1.0 représentant une mesure perceptive de l'intensité et de l'activité. En général, les musiques énergiques semblent rapides, fortes et bruyantes.
   Varibale float entre 0 et 1


7- **instrumentalness (Instrumentalité) :**
   - Détermine si une musique ne contient pas de voix.
Les sons "Ooh" et "aah" sont considérés comme instrumentaux dans ce contexte. Les morceaux de rap ou de musique parlée sont clairement "vocaux". Plus la valeur de l'instrumentalité est proche de 1,0, plus il est probable que la piste ne contienne pas de contenu vocal. Les valeurs supérieures à 0,5 sont censées représenter des titres instrumentaux, mais la confiance est d'autant plus grande que la valeur s'approche de 1,0.
   Varibale float entre 0 et 1


8- **loudness (Loudness) :**
   - Le volume global d'une musique en décibels (dB). Les valeurs de loudness sont moyennées sur l'ensemble de la musique et sont utiles pour comparer le volume relatif des musiques.
   Les valeurs se situent entre -60 et 0 db.

9- **speechiness (Parlantéité) :**
    - Détecte la présence de paroles parlées dans une piste. Plus la valeur de speechiness est proche de 1.0, plus l'enregistrement ressemble exclusivement à des paroles parlées.
       Varibale float entre 0 et 1

10- **liveness (Vivacité) :**
    - Détecte la présence d'un public dans l'enregistrement. Des valeurs de "liveness" plus élevées représentent une probabilité plus grande que la chanson ait été jouée en direct.
       Varibale float entre 0 et 1


11- **Valence (Valence audio) :**
    - Une mesure de 0.0 à 1.0 décrivant la positivité musicale transmise par une musique. Les musiques avec une valence élevée sonnent plus positives, tandis que celles avec une valence basse sonnent plus négatives.
       Varibale float entre 0 et 1

12- **Tempo (Tempo) :**
    - Le tempo estimé global d'une musique en battements par minute (BPM). En terminologie musicale, le tempo est la vitesse ou le rythme d'une pièce donnée et découle directement de la durée moyenne d'un battement.
       Varibale float positive

13- **Popularity (Popularité de la chanson) :**
    - La popularité d'une chanson. C'est une valeur entre 0 et 100 avec 100 étant la plus populaire.


# Etapes du projet
## I - Récupération des données

1-  Scrapping des titres des musiques et leurs artistes entre 2010 et 2023 du site web : https://www.songfacts.com/browse/years/

En utilisant l'API spotify on effectue ce qui suit : 

2-  Récupération de l'identifiant des musiques .

3-  Récupération des caractéristiques audios des musiques à partir de leur identifiant.

4-  Récupération de la popularité de chaque musique.
## II - Prise en main de la base de données

1- Nettoyage de la base de données

2- Analyse exploratoire des données

3- Choix des variables
## III- Modélisation 

1- Régression Linéaire

2- Régression de Ridge

3- Régression Random Forest 

4- Régression Gradient Boosting
## Solution 