<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Larry Wigington's academic portfolio">
    <title>Larry Wigington</title>
    <script>
        // Create favicon
        var canvas = document.createElement('canvas');
        canvas.height = 64;
        canvas.width = 64;
        var context = canvas.getContext('2d');
        context.font = '48px serif';
        context.fillText('L', 8, 48);

        var link = document.createElement('link');
        link.type = 'image/x-icon';
        link.rel = 'icon';
        link.href = canvas.toDataURL("image/png");
        document.head.appendChild(link);
    </script>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 2rem;
            background-color: #fff;
            color: #333;
        }

        header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-top: 5rem;
            margin-bottom: 3rem;
            max-width: 18cm;
            margin: 0 auto;
        }

        .header-text {
            display: flex;
            margin-top: 1.5rem;
            flex-direction: column;
        }

        header h1 {
            font-size: 2.5rem;
            margin: 0;
            line-height: 1.1;
        }

        header .sub-header {
            margin-top: 10px;
            font-size: 1.2rem;
            color: #333;
        }

        .profile-pic {
            max-width: 160px;
            height: auto;
            border-radius: 50%;
        }

        /* Placeholder for profile picture */
        .profile-placeholder {
            width: 160px;
            height: 160px;
            border-radius: 50%;
            background-color: #007BFF;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 4rem;
            font-weight: bold;
        }

        nav {
            margin-bottom: 1.5rem;
            max-width: 18cm;
            margin: 0 auto;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
            margin-top: 2rem;
        }

        nav ul li {
            display: inline-block;
            margin-right: 1rem;
            padding-bottom: 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: #007BFF;
            font-weight: bold;
        }

        nav ul li a:hover {
            text-decoration: underline;
        }

        main {
            max-width: 18cm;
            margin: 0 auto;
        }

        section {
            margin-bottom: 2rem;
        }

        section#about {
            margin-top: 3rem;
        }

        section h1 {
            font-size: 1.8rem;
            margin-top: 1rem;
        }

        section h2 {
            font-size: 1.5rem;
        }

        section p,
        ul {
            font-size: 1rem;
            margin-bottom: 1rem;
        }

        section ul {
            padding-left: 1.2rem;
        }

        section ul li {
            margin-bottom: 1rem;
        }

        a {
            color: #007BFF;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }

        .external-link::after {
            content: "\2197";
            font-size: 0.6em;
            vertical-align: super;
            margin-left: 3px;
        }

        .quote-footer {
            margin-top: 3rem;
            padding-top: 2rem;
            border-top: 1px solid #eee;
            text-align: center;
            font-style: italic;
            color: #666;
        }

        @media (max-width: 600px) {
            .profile-pic,
            .profile-placeholder {
                max-width: 100px;
                width: 100px;
                height: 100px;
                font-size: 3rem;
            }

            header .sub-header {
                font-size: 1rem;
            }

            .header-text {
                margin-top: 0.5rem;
            }

            header h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>

<body>

    <header>
        <div class="header-text">
            <h1>Larry Wigington</h1>
            <p class="sub-header">PhD Student, Operations Research, Naval Postgraduate School</p>
        </div>
        <!-- Replace this div with an img tag when you have your photo -->
        <!-- <img src="profile.jpg" alt="Larry Wigington's Headshot" class="profile-pic"> -->
        <div class="profile-placeholder">LW</div>
    </header>

    <main>
        <nav>
            <ul>
                <li><a href="mailto:lwwiging@nps.edu" class="external-link">Email me</a></li>
                <li><a href="https://github.com/larrywigington" target="_blank" class="external-link">GitHub</a></li>
                <li><a href="https://www.linkedin.com/in/larrywigington" target="_blank" class="external-link">LinkedIn</a></li>
            </ul>
        </nav>

        <section id="about">
            <h1>About</h1>
            <p>
                I am a PhD student in Operations Research at the Naval Postgraduate School,
                advised by <a href="#" target="_blank">Robert Bassett</a>.
                My research focuses on developing GPU-accelerated solvers for stochastic linear programs 
                and large-scale optimization problems. I'm particularly interested in numerical linear algebra, 
                distributed scientific computing, and building educational platforms that make complex 
                mathematical concepts accessible through visualization.
            </p>
        </section>

        <section>
            <h2>Publications & Presentations</h2>
            <ul>
                <li>
                    L. Wigington. Solving Stochastic Programs with GPUs: A Literature Review.
                    <em>International Conference on Stochastic Programming (ICSP)</em>, 2025. <br>
                    <a href="#" target="_blank">📊 Slides</a>
                </li>
                <li>
                    L. Wigington. Solving Stochastic Linear Programs on GPUs.
                    <em>SIAM Northern and Central California Sectional Conference (NCC25)</em>, 2025. <br>
                    <a href="#" target="_blank">📊 Poster</a>
                </li>
            </ul>
        </section>

        <section>
            <h2>Software</h2>
            <p>
                I actively contribute to open-source projects in Python, CUDA, and the scientific computing ecosystem.
                Notable projects include <a href="https://github.com/larrywigington/terminal-assistant" target="_blank">Terminal Assistant</a>,
                an Ollama-based CLI tool for terminal commands, <a href="https://github.com/larrywigington/nla-visualize" target="_blank">NLA-Visualize</a> for
                animated GPU/CPU visualizations of numerical algorithms, and <a href="https://github.com/larrywigington/nla-teaching-notebooks" target="_blank">NLA-Teaching-Notebooks</a> featuring
                educational Jupyter notebooks with clear theory and reproducible examples.
            </p>
        </section>

        <section>
            <h2>Teaching</h2>
            <p>
                I am passionate about making complex mathematical concepts accessible through
                clear explanations and interactive visualizations. I develop educational
                materials and contribute to open-source teaching resources in optimization
                and numerical methods.
            </p>
        </section>

        <div class="quote-footer">
            "Optimization isn't just about better answers — it's about better decisions, faster."
        </div>
    </main>

</body>

</html>
