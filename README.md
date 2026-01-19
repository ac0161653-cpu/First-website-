<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Piyush Chouhan | Student</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Dark themed front page -->
    <div class="front-page">
        <h1>Piyush Chouhan</h1>
        <p>Student | B.Tech CSE (AIML)</p>

        <!-- Buttons to show sections -->
        <div class="buttons">
            <button onclick="showSection('about')">About Me</button>
            <button onclick="showSection('education')">Education</button>
            <button onclick="showSection('skills')">Skills</button>
            <button onclick="showSection('contact')">Contact</button>
        </div>
    </div>

    <!-- Hidden Sections -->
    <section id="about" class="hidden-section">
        <h2>About Me</h2>
        <p>
            I am a first year B.Tech CSE (AIML) student at Shri Vaishnav
            Vidya Peeth Vishwavidyalaya. I am interested in programming
            and learning new technologies related to computer science.
        </p>
    </section>

    <section id="education" class="hidden-section">
        <h2>Education</h2>
        <p>
            <strong>Course:</strong> B.Tech CSE (AIML)<br>
            <strong>University:</strong> Shri Vaishnav Vidya Peeth Vishwavidyalaya<br>
            <strong>Year:</strong> First Year
        </p>
    </section>

    <section id="skills" class="hidden-section">
        <h2>Skills</h2>
        <ul>
            <li>Python</li>
            <li>HTML</li>
        </ul>
    </section>

    <section id="contact" class="hidden-section">
        <h2>Contact</h2>
        <p>Email: <a href="mailto:ac0161653@gmail.com">ac0161653@gmail.com</a></p>
    </section>

    <footer>
        <p>© 2026 Piyush Chouhan</p>
    </footer>

    <script>
        function showSection(id) {
            // Hide all sections
            const sections = document.querySelectorAll('.hidden-section');
            sections.forEach(sec => sec.style.display = 'none');

            // Show clicked section
            document.getElementById(id).style.display = 'block';
        }
    </script>

</body>
</html>
