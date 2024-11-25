<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>My Projects</title>
    <style>
        /* General Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body and Layout */
        body {
            font-family: 'Arial', sans-serif;
            background-color: #121212; /* Dark background similar to Spotify */
            color: #e0e0e0; /* Light gray text */
        }

        /* Header Styling */
        header {
            background: linear-gradient(to right, #1db954, #1ed760); /* Spotify's signature gradient */
            padding: 60px 0;
            text-align: center;
        }

        .header-content h1 {
            font-size: 3rem;
            color: white;
            margin-bottom: 10px;
        }

        .header-content p {
            font-size: 1.2rem;
            color: #d1d1d1;
        }

        /* Projects Section */
        #projects {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)); /* Grid layout for project cards */
            gap: 40px;
            padding: 40px;
        }

        /* Individual Project Cards */
        .project-card {
            background-color: #181818; /* Dark card background */
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-10px); /* Hover effect for cards */
        }

        .project-image img {
            width: 100%;
            height: auto;
            border-bottom: 4px solid #1db954; /* Green accent on bottom */
        }

        /* Project Details */
        .project-details {
            padding: 20px;
        }

        .project-details h2 {
            font-size: 1.8rem;
            color: #1db954; /* Spotify green */
            margin-bottom: 10px;
        }

        .project-details p {
            font-size: 1.1rem;
            color: #b3b3b3; /* Light gray text for project description */
            margin-bottom: 20px;
        }

        /* Video Container Styling */
        .video-container {
            position: relative;
            padding-bottom: 56.25%; /* 16:9 aspect ratio */
            height: 0;
            overflow: hidden;
            max-width: 100%;
            border-radius: 10px;
            background-color: #000;
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }

        /* Footer Styling */
        footer {
            background-color: #181818;
            padding: 20px 0;
            text-align: center;
        }

        footer p {
            font-size: 1rem;
            color: #b3b3b3;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header-content h1 {
                font-size: 2.5rem;
            }

            .project-details h2 {
                font-size: 1.5rem;
            }

            .project-details p {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="header-content">
            <h1>My Projects</h1>
            <p>Explore my work, including images, videos, and descriptions.</p>
        </div>
    </header>

    <section id="projects">
        <div class="project-card">
            <div class="project-image">
                <img src="project1.jpg" alt="Project 1 Image">
            </div>
            <div class="project-details">
                <h2>Project Title 1</h2>
                <p>A short description of this project. This project features interactive design and modern techniques.</p>
                <div class="video-container">
                    <iframe src="https://www.youtube.com/embed/your_video_id" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>
        </div>

        <div class="project-card">
            <div class="project-image">
                <img src="project2.jpg" alt="Project 2 Image">
            </div>
            <div class="project-details">
                <h2>Project Title 2</h2>
                <p>Another innovative project featuring advanced functionality and beautiful user interface design.</p>
                <div class="video-container">
                    <iframe src="https://www.youtube.com/embed/your_video_id" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="footer-content">
            <p>&copy; 2024 My Portfolio. All Rights Reserved.</p>
        </div>
    </footer>
</body>
</html>
