<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Votre Page Sociale</title>
    <style>
        body {
            font-family: 'ꓚ⌊⌋', sans-serif;
            background-color: #f5f5dc; /* Couleur beige pour le fond */
            background-image: url('https://th.bing.com/th/id/OIP.N2RtaUxZEB04j_ukSzNXlAAAAA?rs=1&pid=ImgDetMain');
            background-size: 3%;
            background-position: center;
            text-align: center;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh; /* Ajusté à min-height pour garantir une hauteur minimale sur les appareils mobiles */
            color: #333; /* Couleur de texte */
        }

        h1 {
            color: #000000; /* Couleur différente pour le titre */
            font-size: 28px; /* Taille différente pour le titre */
            margin-bottom: 15px; /* Ajout de marge en bas */
        }

        .profile-link {
            color: #ffffff; /* Couleur du texte pour les liens */
            text-decoration: none;
        }

        .social-links {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: space-between;
            width: 80%;
            margin-top: 15px; /* Ajusté pour réduire l'espace entre le titre et les liens */
        }

        .profile-link {
            flex: 1;
            width: 100%;
            margin: 10px 0;
            padding: 12px 20px; /* Ajusté pour réduire la taille des liens */
            background-color: #000000; /* Couleur de fond pour les liens */
            border-radius: 5px;
        }

        @media (max-width: 768px) {
            body {
                background-size: 100%;
            }
            .social-links {
                width: 100%;
            }
        }
    </style>
</head>
<body>
    <h1>Voici les réseaux de Maison Singulière</h1>

    <!-- Liens pour Instagram et Facebook -->
    <div class="social-links">
        <a href="https://www.instagram.com/maisonsinguliere_deco?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==" class="profile-link" target="_blank">Instagram</a>
        <a href="https://www.facebook.com/profile.php?id=100085934167461" class="profile-link" target="_blank">Facebook</a>
    </div>
</body>
</html>


