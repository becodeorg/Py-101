# Python 101

# D5 - Fun projects

### Installez les packages avec Pip

Pip est un gestionnaire de packages Python.

```shell
pip install <package>
```

Afficher les packets déjà télécharger

```shell
pip freeze
```

## Web scraping avec Requests et Beautifull_soup

ETL signifie extraction, transformation et chargement (Extract, Transform, Load en anglais). C'est une procédure qui "permettant d'effectuer des synchronisations massives d'information d'une source de données (le plus souvent une base de données) vers une autre" (source [Wikipédia](https://fr.wikipedia.org/wiki/Extract-transform-load)).

```shell
pip install requests
```

```shell
pip install beautifulsoup4
```

```py

# On importe requests
import requests
# On importe beautifulsoup
from bs4 import BeautifulSoup as bs

# On défini l'url du site
url = "https://www.gov.uk/search/news-and-communications"
# On utilise la fonction get() du package requests
page = requests.get(url)
soup = bs(page.content, 'html.parser')
# On utilise beautifulsoup pour aller chercher les balises a avec la classe "gem-c-document-list__item-title"
titres_bs = soup.find_all("a", class_="gem-c-document-list__item-title")
# On utilise beautifulsoup pour aller chercher les balises a avec la classe "gem-c-document-list__item-title"
descriptions_bs = soup.find_all(
    "p", class_="gem-c-document-list__item-description")
# On utilise beautifulsoup pour aller chercher les balises p avec la classe "gem-c-document-list__item-description"

titres = []
# On initie des listes vides

descriptions = []
# On initie des listes vides

for titre in titres_bs:
    # print(titre.string)
    titres.append(titre.string)

# On boucle et on push dans notre liste

for index, description in enumerate(descriptions_bs):
    descriptions.append((index, description.string))

# On boucle et on push dans notre liste

print(titres[0],':', descriptions[0][1], end='\r')

```

## Détection de visage avec openCV et DeepFace

On va utiliser les fichiers .xml fournit par open CV pour détecter des visages dans des images.

```shell
pip install opencv-python
```

```shell
pip install pathlib2
```

```py

from deepface import DeepFace
import pathlib
import cv2

cascade_path = pathlib.Path(cv2.__file__).parent.absolute(
)/"data/haarcascade_frontalface_default.xml"  # Path du modèle dans l'objet

# Classifier
clf = cv2.CascadeClassifier(str(cascade_path))

# camera= cv2.VideoCapture("people.mp4") - On peut aussi utiliser le programe sur une vidéo
camera = cv2.VideoCapture(0)

# Boucle infinie de génération des frames
while True:
    _, frame = camera.read()
    # Conversion des images en niveau de gris
    gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)

    faces = clf.detectMultiScale(
        gray,
        scaleFactor=1.1,
        minNeighbors=5,
        minSize=(30, 30),
        flags=cv2.CASCADE_SCALE_IMAGE
    )

    for (x, y, width, height) in faces:
        cv2.rectangle(frame, (x, y), (x+width, y+height), (255, 255, 3), 2)
        try:
            analyze = DeepFace.analyze(
                frame, actions=['age', 'gender', 'race', 'emotion'])
            print(analyze)
        except:
            print("no face")

    cv2.imshow("Faces", frame)

    if cv2.waitKey(1) == ord("q"):
        break

camera.release()
cv2.destroyAllWindows()
```
