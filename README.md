<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zaqee's Bio</title>
    <style>
        /* Add your custom CSS styles here */
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .container {
            text-align: center;
            animation: fadeIn 1s ease-in-out;
        }

        .animated-text {
            font-size: 3rem;
            color: #ff7e5f;
            text-transform: uppercase;
            font-weight: bold;
        }

        .button {
            display: inline-block;
            padding: 10px 20px;
            margin-top: 20px;
            background-color: #ff7e5f;
            color: #fff;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .button:hover {
            background-color: #ff6b49;
        }

        .social-links {
            margin-top: 50px;
        }

        .social-link {
            display: inline-block;
            margin: 0 10px;
        }

        .projects {
            margin-top: 50px;
        }

        .project {
            display: inline-block;
            margin: 0 10px;
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="animated-text" id="animatedText">
            <span>Z</span>
            <span>a</span>
            <span>q</span>
            <span>e</span>
            <span>e</span>
        </div>
        <div class="social-links">
            <a href="https://twitter.com/your_username" class="social-link">
                <img src="https://img.shields.io/twitter/follow/your_username?style=social" alt="Twitter">
            </a>
            <a href="https://www.linkedin.com/in/your_username" class="social-link">
                <img src="https://img.shields.io/badge/LinkedIn-Connect-blue" alt="LinkedIn">
            </a>
            <a href="mailto:your.email@example.com" class="social-link">
                <img src="https://img.shields.io/badge/Email-Send-red" alt="Email">
            </a>
        </div>
        <a href="#" class="button">View Projects</a>
        <div class="projects">
            <!-- Showcase of your projects -->
            <div class="project">
                <img src="project1_thumbnail.jpg" alt="Project 1">
                <p>Project 1 Description</p>
            </div>
            <div class="project">
                <img src="project2_thumbnail.jpg" alt="Project 2">
                <p>Project 2 Description</p>
            </div>
            <div class="project">
                <img src="project3_thumbnail.jpg" alt="Project 3">
                <p>Project 3 Description</p>
            </div>
        </div>
    </div>

    <script>
        // Animation for the name
        const animatedText = document.getElementById('animatedText');
        const characters = animatedText.querySelectorAll('span');
        let index = 0;

        function animateName() {
            characters[index].classList.add('fadeInLeft');
            index++;
            if (index < characters.length) {
                setTimeout(animateName, 200);
            }
        }

        animateName();
    </script>
</body>

</html>