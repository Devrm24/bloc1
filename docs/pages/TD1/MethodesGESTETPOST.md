### ALEXANDRE SIMSEK TD1

# Différence en methode  **GET** et **POST**

## Methode **GET**


**Avec la méthode GET** les données sont écrites `directement dans l’URL`.

__EXEMPLE__:

www.example.com/register.php?firstname=peter&name=miller&age=55&gender=male

  _ici les paramètres sont affichés avec l'URL_

__Cela presente des  **avantages** et **inconvénients**__  


* __Avantage__
  -  Les paramètres de l’URL peuvent être enregistrés avec l’adresse du site Web.
 


* __Inconvénients__
  -  Le principal inconvénient de la méthode GET est l’absence de protection des données.
       Les paramètres URL sont alors visibles dans la barre d'adresse et stockés sans chiffrement dans l’historique du navigateur

  -  Un deuxième inconvénient est sa capacité limitée l’URL ne peut pas contenir plus de 2 000 caractères environ.
        De plus les paramètres des URL ne peuvent pas contenir des caractères ASCII


## Méthode **POST**     

__La méthode POST__ écrit les paramètres `URL dans la requête HTTP` pour le serveur.

* __Avantage__
Les paramètres ne sont donc pas visibles pour les utilisateurs et la portée des requêtes POST est illimitée.
La méthode POST permet de garder la confidentialité nécessaire. Les données ne sont pas mises en cache et n’apparaissent pas dans l’historique de navigation.


* __Inconvénients__
 Si une page Web est mise à jour avec un formulaire dans le navigateur (par exemple, en utilisant le bouton « Précédent » / « Retour »), les données du formulaire doivent être de nouveau soumises 



## 2)


| **GET**                                   | **POST**                                 |
|---------------------------------------|---------------------------------------|
| Les données sont visibles dans l'URL  | Les données ne sont pas visibles      |
| Limité par la longueur de l'URL       | Pas de limite spécifique              |
| Récupération de données               | Envoi de données au serveur           |
| Moins sécurisé pour les données sensibles | Plus sécurisé pour les données sensibles |
| Les réponses peuvent être mises en cache | Les réponses ne sont généralement pas mises en cache |

Lien utilisé :https://www.ionos.fr/digitalguide/sites-internet/developpement-web/get-vs-post/

## 3)

Le protocole HTTP est extensible grâce :

- Méthodes **HTTP** : Nouvelles méthodes comme `PATCH` peuvent être ajoutées.
- En-têtes **HTTP** : Les en-têtes personnalisés permettent de transmettre des informations spécifiques.
- Évolutions : HTTP/2 et HTTP/3 ajoutent des fonctionnalités comme la multiplexation, tout en étant rétrocompatibles.
- Sécurité : Intégration de nouvelles normes de sécurité, comme `TLS` pour HTTPS.

  Cette flexibilité permet à HTTP de s’adapter aux évolutions du web.

 ## 4)

  En informatique, un protocole sans état (_en anglais stateless protocol_)
  est un protocole de communication qui n'enregistre pas l'état d'une session de communication entre deux requêtes successives.

  Le **HTTP** améliore la sécurité et l'extensibilité , mais nécessite des mécanismes supplémentaires pour gérer la continuité de la navigation et des interactions utilisateur sur le Web.

## 5)

<img src="https://www.aurone.com/wp-content/uploads/blog/inline/images/anatomie-dune-url-siteweb.jpg" alt="URL Décomposition" width="400" height="400"> 

### **PROTOCOLE** 
Un protocole est un ensemble de règles qui définissent comment les données doivent être échangées entre systèmes pour permettre une communication correcte et compréhensible.

### **SOUS DOMAINE** 
Un sous-domaine est une partie d'un domaine principal dans un système de nommage. Par exemple, dans blog.example.com, blog est un sous-domaine de example.com.

### **DOMAINE**
Un domaine est une adresse sur Internet, comme example.com, utilisée pour identifier un site web ou un service en ligne.

### **EXTENSION**  <img src="https://www.apyart.com/3853-large_default/bleu-pastel-clair.jpg" alt="BLEU CLAIR" width="20" height="20"> 
Une extension est une partie ajoutée à un nom de domaine, comme .com ou .org, qui indique le type ou la localisation du site web.


### **SOUS DOSSIERS** 
Un sous-dossier est un dossier situé à l'intérieur d'un autre dossier, permettant d'organiser les fichiers de manière hiérarchique.

### **SLUG** 
Un slug est une version simplifiée et lisible d'une URL, généralement utilisée pour identifier une page ou un article de manière claire et concise, souvent en remplaçant les espaces par des tirets.


## 6)
* __Les **fammilles** de code status de la réponse HTTP entre le client et serveur sont:__
  - (1xx) réponse informationnelle
  - (2xx) succès
  - (3xx) redirection
  - (4xx) erreur client
  - (5xx) erreur serveur

## 7)
En `HTTP`, la négociation de contenu est le mécanisme utilisé pour servir différentes représentations d'une ressource à partir du même URI, 
pour aider l'agent utilisateur à indiquer la représentation la plus adaptée à l'utilisatrice ou à l'utilisateur par exemple : la langue du document, le format d'image ou l'encodage à utiliser pour le contenu).

<img src="https://developer.mozilla.org/fr/docs/Web/HTTP/Content_negotiation/httpnego.png" alt="NEGOCIATION CONTENUE SCHEMA" width="450" height="300"> _schéma la négociation de contenu_
