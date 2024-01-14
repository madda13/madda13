<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sélectionner un réseau social</title>
    
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background-color: #f4f4f4; /* Ajoutez une couleur de fond si nécessaire */
        }

        .container {
            text-align: center;
            margin-top: 50px;
        }

        h1 {
            color: #333; /* Couleur du texte pour le titre */
        }

        button {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            background-color: #3498db; /* Couleur de fond du bouton */
            color: #fff; /* Couleur du texte du bouton */
            border: none;
            border-radius: 5px;
        }

        button:hover {
            background-color: #2980b9; /* Couleur de fond au survol du bouton */
        }

        #qrcode {
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Choisissez un réseau social</h1>
        <button onclick="redirigerVers('instagram')">Instagram</button>
        <button onclick="redirigerVers('facebook')">Facebook</button>
        <div id="qrcode"></div>
    </div>

    <script src="https://cdn.rawgit.com/davidshimjs/qrcodejs/gh-pages/qrcode.min.js"></script>
    <script>
        // Fonction pour rediriger vers l'URL appropriée
        function redirigerVers(reseauSocial) {
            let url;

            if (reseauSocial === 'instagram') {
                url = "https://www.instagram.com/votre_nom_utilisateur_instagram/";
            } else if (reseauSocial === 'facebook') {
                url = "https://www.facebook.com/votre_nom_utilisateur_facebook/";
            }

            window.location.href = url;
        }

        // Générer le QR code avec le contenu de la page actuelle
        const qrcode = new QRCode(document.getElementById("qrcode"), {
            text: document.documentElement.outerHTML, // Utilisez le contenu HTML de la page
            width: 200,
            height: 200
        });
    </script>
</body>
</html>
