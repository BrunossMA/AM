<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Andrea Mauro Portfolio - #AM</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/4.5.2/css/bootstrap.min.css">
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        .container {
            margin-top: 50px;
        }
        h1, h2 {
            text-align: center;
            color: #007BFF;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Andrea Mauro - Portfolio #AM</h1>
        <p class="text-center">Benvenuti nel portfolio di Andrea Mauro. Qui troverete una panoramica dei suoi progetti e statistiche rilevanti.</p>

        <!-- Sezione Progetti -->
        <h2>Progetti Principali</h2>
        <ul>
            <li><a href="https://github.com/andreamauro/progetto1" target="_blank">Progetto 1</a></li>
            <li><a href="https://github.com/andreamauro/progetto2" target="_blank">Progetto 2</a></li>
            <li><a href="https://github.com/andreamauro/progetto3" target="_blank">Progetto 3</a></li>
        </ul>

        <!-- Sezione Statistiche -->
        <h2>Statistiche GitHub</h2>
        <div id="stats" class="text-center">
            <p>Caricamento delle statistiche in corso...</p>
        </div>
    </div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script>
        $(document).ready(function() {
            // Caricare le statistiche GitHub per Andrea Mauro
            fetch('https://api.github.com/users/andreamauro')
            .then(response => response.json())
            .then(data => {
                $('#stats').html(`
                    <p><strong>Username:</strong> ${data.login}</p>
                    <p><strong>Numero di Repository Pubblici:</strong> ${data.public_repos}</p>
                    <p><strong>Follower:</strong> ${data.followers}</p>
                    <p><strong>Seguiti:</strong> ${data.following}</p>
                `);
            })
            .catch(error => {
                $('#stats').html('<p>Errore nel caricamento delle statistiche.</p>');
            });
        });
    </script>
</body>
</html>
