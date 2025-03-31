# Biblioteca-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Biblioteca - Your Study Hub</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #f4f4f4;
            color: #333;
            text-align: center;
            transition: background 0.3s, color 0.3s;
        }

        header {
            background: #007bff;
            color: white;
            padding: 15px;
            text-align: center;
        }

        .nav-links {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        .nav-links li {
            display: inline;
        }

        .nav-links a {
            text-decoration: none;
            color: white;
            font-size: 18px;
            padding: 10px;
        }

        .hero {
            padding: 50px;
        }

        .cta-button {
            background: #28a745;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 18px;
            cursor: pointer;
        }

        .cta-button:hover {
            background: #218838;
        }

        footer {
            margin-top: 20px;
            padding: 10px;
            background: #007bff;
            color: white;
        }

        #darkModeToggle {
            background: black;
            color: white;
            border: none;
            padding: 5px 10px;
            cursor: pointer;
        }

        #darkModeToggle:hover {
            background: gray;
        }

        .dark-mode {
            background: #333;
            color: white;
        }
    </style>
    <script defer>
        // Dark Mode Toggle Functionality
        document.addEventListener("DOMContentLoaded", () => {
            const darkModeToggle = document.getElementById("darkModeToggle");
            darkModeToggle.addEventListener("click", () => {
                document.body.classList.toggle("dark-mode");
            });
        });

        // Search Functionality (Basic Example)
        document.addEventListener("DOMContentLoaded", () => {
            const searchBox = document.getElementById("searchBox");
            searchBox.addEventListener("keyup", (event) => {
                let query = event.target.value.toLowerCase();
                console.log("Searching for:", query);
            });
        });
    </script>
</head>
<body>
    <header>
        <nav>
            <div class="logo">Biblioteca</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#notes">Notes</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><button id="darkModeToggle">Dark Mode</button></li>
            </ul>
        </nav>
    </header>
    
    <section id="home" class="hero">
        <h1>Welcome to Biblioteca</h1>
        <p>Your ultimate study material hub.</p>
        <input type="text" id="searchBox" placeholder="Search your notes...">
        <button class="cta-button">Explore Notes</button>
    </section>

    <footer>
        <p>&copy; 2025 Biblioteca. All Rights Reserved.</p>
    </footer>
</body>
</html>
