<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Andrea Mauro's Portfolio</title>
    <!-- Import Roboto font from Google Fonts -->
    <link href="https://fonts.googleapis.com/css?family=Roboto:400,700&display=swap" rel="stylesheet"> 
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
            background-color: #f7f7f7; /* Light background for minimalism */
        }
        header {
            background-color: #ffffff;
            color: #333;
            padding: 40px 20px;
            text-align: center;
            border-bottom: 1px solid #e0e0e0;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
            font-weight: 700;
        }
        .container {
            max-width: 800px;
            margin: 40px auto;
            padding: 0 20px;
        }
        h2 {
            color: #333;
            font-size: 1.8em;
            margin-bottom: 20px;
            font-weight: 700;
        }
        p {
            font-size: 1em;
            line-height: 1.6;
            margin-bottom: 20px;
        }
        .grid {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }
        .project-card {
            flex: 1 1 calc(33% - 20px);
            background-color: #ffffff;
            padding: 20px;
            text-decoration: none;
            color: #333;
            border: 1px solid #e0e0e0;
            border-radius: 5px;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.08);
        }
        .project-card h3 {
            margin-top: 0;
            font-size: 1.2em;
            font-weight: 700;
        }
        .project-card span {
            display: block;
            font-size: 0.9em;
            color: #666;
            margin-top: 10px;
        }
        footer {
            background-color: #ffffff;
            color: #999;
            text-align: center;
            padding: 20px;
            border-top: 1px solid #e0e0e0;
            margin-top: 40px;
        }
        a {
            color: #1a0dab;
        }
        a:hover {
            text-decoration: underline;
        }
        @media (max-width: 768px) {
            .project-card {
                flex: 1 1 100%;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Andrea Mauro's Portfolio</h1>
</header>

<div class="container">
    <h2>About Me</h2>
    <p>Hi everyone, nice to meet you! I’m Andrea, and this is a page where I collect my personal projects. Hope you like it, and if you have any advice, feel free to let me know!</p>
</div>

<div class="container">
    <h2>Projects</h2>
    <div class="grid">
        <a href="https://github.com/your-username/project1" target="_blank" class="project-card">
            <h3>Project 1</h3>
            <span>Financial risk analysis using statistical models for portfolio optimization.</span>
        </a>
        <a href="https://github.com/your-username/project2" target="_blank" class="project-card">
            <h3>Project 2</h3>
            <span>Study of economic variables through multiple regressions for future market forecasting.</span>
        </a>
        <a href="https://github.com/your-username/project3" target="_blank" class="project-card">
            <h3>Project 3</h3>
            <span>Implementation of a machine learning model for credit risk prediction.</span>
        </a>
        <!-- Add more project cards as needed -->
    </div>
</div>

<div class="container">
    <h2>Contact</h2>
    <p>Email: <a href="mailto:youremail@example.com">youremail@example.com</a></p>
    <p>LinkedIn: <a href="https://www.linkedin.com/in/your-username" target="_blank">linkedin.com/in/your-username</a></p>
</div>

<footer>
    &copy; 2024 Andrea Mauro - All rights reserved
</footer>

</body>
</html>
