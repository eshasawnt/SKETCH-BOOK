# SKETCH-BOOK
FINAL MODULE.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My E-Book</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            transition: background 0.3s, color 0.3s;
            background: #FFC0CB;
            color: black;
        }

        .hidden { display: none; }

        .navbar {
            background: rgba(0, 0, 0, 0.7);
            color: white;
            font-style: italic;
            display: flex;
            justify-content: center;
            padding: 5px 0;
            font-size: 18px;
        }
        .navbar a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            padding: 5px;
        }
        .navbar a:hover {
            text-decoration: underline;
        }

        #welcome-screen {
            margin-top: 10%;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(7, 20px);
            grid-template-rows: repeat(6, 20px);
            gap: 2px;
            margin-top: 20px;
            justify-content: center;
        }
        .pixel, .blue, .petal, .center {
            width: 20px;
            height: 20px;
        }
        .pixel {
            background: transparent;
        }
        .blue {
            background: white;
        }

        #flipbook {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            margin: 10px auto;
            width: 60%;
            background: white;
            border-radius: 25px;
            box-shadow: 0 0 20px rgba(0,0,0,0.2);
            padding: 40px;
        }

        .page {
            
            width: 80%;
            height: 100%;
            overflow-y: auto;
            display: none;
            flex-direction: column;
            justify-content: center;
            min-height: 90vh;
           max-width: 600px;
          margin: auto;
            padding: 40px;
          align-items: center;
            text-align: left;
            background: white;
            color: black;
            border-radius: 15px;
        }

        .page.active { display: block; }

        .button-container {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 20px auto;
        }

        button {
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            background: #007BFF;
            color: white;
            border-radius: 5px;
        }
        button:hover {
            background: #0056b3;
        }

        .dark-mode {
            background: #222;
            color: white;
        }

        .dark-mode #flipbook, .dark-mode .page {
            background: #333;
            color: white;
            border-color: #555;
        }

        .centered-title {
            text-align: center;
            font-weight: bold;
            font-style: italic;
        }
    </style>
</head>
<body>
    <div class="navbar">
        <a href="home2.html">Home</a>
        <a href="about2.html">About</a>
    </div>

    <div id="welcome-screen">
        <!-- Pixel Heart -->
        <div class="grid">
            <div class="pixel"></div><div class="blue"></div><div class="blue"></div><div class="pixel"></div><div class="blue"></div><div class="blue"></div><div class="pixel"></div>
            <div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div>
            <div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div>
            <div class="pixel"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="pixel"></div>
            <div class="pixel"></div><div class="pixel"></div><div class="blue"></div><div class="blue"></div><div class="blue"></div><div class="pixel"></div><div class="pixel"></div>
            <div class="pixel"></div><div class="pixel"></div><div class="pixel"></div><div class="blue"></div><div class="pixel"></div><div class="pixel"></div><div class="pixel"></div>
        </div>
        <h2>Enter your name:</h2>
        <input type="text" id="username" placeholder="Your name">
        <button id="start-btn">Start Reading</button>
    </div>

    <div id="ebook-container" class="hidden">
        <h1 id="welcome-message"></h1>
        <button id="dark-mode-btn">🌙 Bright OR Dark Mode ☀️</button><br>
        <div class="centered-title">lets read !!</div><br>

        <div class="page active">
            <h2 class="centered-title">THE SKETCHBOOK<h6 class="centered-title">(PART:1) SKETCHING HER IN SILENCE</h2></h6><br><br>
           <h4 class="centered-title"> 1 : MAYA IN MAYANAGARI</h4><br>
            A sea of lights, moving cars like tiny fireflies, and a chaotic rhythm she had yet to understand. Maya—silent, innocent, and breathtakingly gorgeous, carried a pure soul within her. She had spent her childhood in Texas, America, but now she had arrived in India to complete her higher studies at Bombay University.<br><br>
            It was the rainy season when she first stepped into the bustling campus, the scent of wet earth mixing with the aroma of hot chai from street vendors. The rhythmic downpour mirrored the turbulence inside her—anxiety, excitement, and the nervous energy of stepping into an unfamiliar world.<br><br>
            Her first day was overwhelming. She was unaccustomed to the noise, the fast-paced lifestyle, and the sea of unfamiliar faces...
        </div>
        <div class="page">
            <h2 class="centered-title">THE SKETCHBOOK<h6 class="centered-title">(PART:1) SKETCHING HER IN SILENCE</h2></h6><br><br>
            As she entered her classroom, her eyes scanned the room for an empty seat. She hesitantly sat beside a girl named Riama, who had a stark contrast to Maya’s reserved nature. Riama was an extrovert, talkative, and radiated an easy confidence that made her the center of attention wherever she went.<br><br>
            As soon as Maya settled in, the professor began the lecture. She tried her best to focus, but Riama’s curiosity was unstoppable. She leaned closer, whispering questions.<br><br>
            "Hey, you're new, right? Where are you from? What’s your name? You look like you’re from abroad!"<br><br>
            Maya hesitated before answering softly, "I’m Maya. I’m from Texas."
        </div>
        <div class="page">
            <h2 class="centered-title">THE SKETCHBOOK<h6 class="centered-title">(PART:1) SKETCHING HER IN SILENCE</h2></h6><br><br>
            "Whoa! Texas? That’s so cool! What’s it like there? Why did you come to Bombay? Do you like Bollywood movies?" Riama continued, her excitement evident.<br><br>
            Maya smiled faintly but gave short responses, feeling slightly uneasy with all the attention. However, her beauty had already made an impact on the class. Boys discreetly stole glances at her, some whispering among themselves, others unable to take their eyes off her. She was oblivious to the effect she had on them, but she could feel the weight of their stares.<br><br>
            As the days passed, Riama took it upon herself to make Maya feel at home. She introduced her to the campus, helped her navigate the chaotic city life, and slowly...
        </div>

        <div class="button-container">
            <button id="prev-btn">Previous</button>
            <button id="next-btn">Next</button>
        </div>
    </div>

    <script>
        document.getElementById("start-btn").addEventListener("click", function() {
            let name = document.getElementById("username").value;
            if (name) {
                document.getElementById("welcome-message").innerText = "Welcome, " + name + "!";
                document.getElementById("welcome-screen").classList.add("hidden");
                document.getElementById("ebook-container").classList.remove("hidden");
            }
        });

        document.getElementById("dark-mode-btn").addEventListener("click", function() {
            document.body.classList.toggle("dark-mode");
            let btn = document.getElementById("dark-mode-btn");
            if (document.body.classList.contains("dark-mode")) {
                btn.innerHTML = "☀️ Light Mode";
            } else {
                btn.innerHTML = "🌙 Dark Mode ";
            }
        });

        let currentPage = 0;
        const pages = document.querySelectorAll(".page");

        function updatePages() {
            pages.forEach((page, index) => {
                page.classList.toggle("active", index === currentPage);
            });
        }

        document.getElementById("prev-btn").addEventListener("click", function() {
            if (currentPage > 0) {
                currentPage--;
                updatePages();
            }
        });

        document.getElementById("next-btn").addEventListener("click", function() {
            if (currentPage < pages.length - 1) {
                currentPage++;
                updatePages();
            }
        });
    </script>
</body>
</html>
