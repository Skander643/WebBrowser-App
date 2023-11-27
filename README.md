
Introduction :
    ETBrowser est une application Android simple qui permet aux utilisateurs de naviguer sur le Web à l'aide d'un WebView intégré. L'application offre des fonctionnalités telles que la navigation vers des URL, le retour en arrière et en avant dans l'historique, le rafraîchissement de la page, la copie de l'URL dans le presse-papiers et le partage de l'URL actuelle.

Fonctionnalités principales: 
  1-Barre d'adresse interactive

  2-Saisissez des URL dans la barre d'adresse et appuyez sur "Go" pour naviguer vers la page Web correspondante.
  3-L'application utilise une expression régulière pour vérifier si l'entrée est une URL valide.
Navigation

  4-Boutons de navigation permettant de revenir en arrière et d'avancer dans l'historique du WebView.
Rafraîchissement de la page

  5-Bouton pour recharger la page actuelle dans le WebView.
Copie d'URL

  6-Icône permettant de copier l'URL actuelle dans le presse-papiers.
Partage d'URL

  7-Icône permettant de partager l'URL actuelle via d'autres applications.
  
Architecture du code :
     Le code source est structuré de manière à suivre les meilleures pratiques de développement Android, en utilisant l'architecture MVC (Modèle-Vue-Contrôleur).

  1-MainActivity : 

  -Activité principale de l'application.
  -Gère l'interface utilisateur et les interactions avec l'utilisateur.
  2-MyWebViewClient

   -Classe interne personnalisée étendant WebViewClient.
   -Contrôle le comportement du WebView, notamment en gérant les événements de chargement de page.

Utilisation des bibliothèques : 
       L'application utilise les fonctionnalités fournies par les bibliothèques Android standard, y compris WebView, EditText, ImageView, et d'autres.

Commentaires dans le code : 
       Le code source est accompagné de commentaires pour expliquer chaque section, méthode et action. Ces commentaires sont destinés à faciliter la compréhension du code et à fournir des indications sur les fonctionnalités spécifiques.

Commentaires spécifiques : 
      La méthode copyToClipboard(String url) utilise un objet ClipData pour copier l'URL dans le presse-papiers. L'étiquette de cet objet utilise un horodatage pour garantir l'unicité et éviter l'écrasement des valeurs précédentes dans le presse-papiers.
      La méthode loadMyUrl(String url) vérifie si l'entrée de l'utilisateur correspond à une URL valide à l'aide de l'expression régulière fournie par Patterns.WEB_URL. Si c'est le cas, l'URL est chargée dans le WebView. Sinon, une recherche Google est effectuée avec la requête saisie.

Conclusion : 
       ETBrowser est une application simple mais fonctionnelle pour la navigation Web sur des appareils Android. Elle met en œuvre des fonctionnalités de base de navigation et offre une expérience utilisateur intuitive.
