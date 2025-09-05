```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Vidyasagar Academy</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0; padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }
        header {
            background-color: #004080;
            color: white;
            padding: 1rem 2rem;
            text-align: center;
        }
        nav {
            background-color: #0066cc;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 1rem 1.5rem;
            display: block;
            font-weight: bold;
            transition: background-color 0.3s ease;
        }
        nav a:hover {
            background-color: #004080;
        }
        main {
            max-width: 900px;
            margin: 2rem auto;
            padding: 0 1rem;
            background-color: white;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            border-radius: 5px;
        }
        h1, h2, h3 {
            color: #004080;
        }
        section {
            margin-bottom: 2rem;
        }
        ul {
            list-style-type: disc;
            margin-left: 1.5rem;
        }
        footer {
            background-color: #004080;
            color: white;
            text-align: center;
            padding: 1rem 2rem;
            margin-top: 3rem;
        }
        form label {
            display: block;
            margin-top: 0.75rem;
            font-weight: bold;
        }
        form input, form textarea, form select {
            width: 100%;
            padding: 0.5rem;
            margin-top: 0.25rem;
            border: 1px solid #ccc;
            border-radius: 3px;
            box-sizing: border-box;
        }
        form button {
            margin-top: 1rem;
            background-color: #0066cc;
            color: white;
            border: none;
            padding: 0.75rem 1.5rem;
            font-size: 1rem;
            border-radius: 3px;
            cursor: pointer;
        }
        form button:hover {
            background-color: #004080;
        }
        /* Simple tab navigation */
        .tab-content {
            display: none;
        }
        .tab-content.active {
            display: block;
        }
        .tabs {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            background-color: #e6f0ff;
            border-radius: 5px 5px 0 0;
            margin-bottom: 1rem;
        }
        .tabs button {
            background: none;
            border: none;
            padding: 1rem 1.5rem;
            cursor: pointer;
            font-weight: bold;
            color: #004080;
            border-bottom: 3px solid transparent;
            transition: border-color 0.3s ease;
        }
        .tabs button.active {
            border-bottom: 3px solid #004080;
            color: #00264d;
        }
        @media (max-width: 600px) {
            nav {
                flex-direction: column;
            }
            nav a {
                padding: 0.75rem 1rem;
            }
            .tabs {
                flex-direction: column;
            }
            .tabs button {
                border-bottom: none;
                border-left: 3px solid transparent;
                padding: 0.75rem 1rem;
            }
            .tabs button.active {
                border-left: 3px solid #004080;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Vidyasagar Academy</h1>
    </header>
    <nav>
        <a href="#home" class="nav-link" data-tab="home">Home</a>
        <a href="#about" class="nav-link" data-tab="about">About Us</a>
        <a href="#academics" class="nav-link" data-tab="academics">Academics</a>
        <a href="#login" class="nav-link" data-tab="login">Login</a>
        <a href="#admissions" class="nav-link" data-tab="admissions">Admissions</a>
        <a href="#studentlife" class="nav-link" data-tab="studentlife">Student Life</a>
        <a href="#resources" class="nav-link" data-tab="resources">Resources</a>
        <a href="#news" class="nav-link" data-tab="news">News and Events</a>
        <a href="#contact" class="nav-link" data-tab="contact">Contact Us</a>
    </nav>
    <main>
        <!-- Home -->
        <section id="home" class="tab-content active">
            <h2>Welcome to Vidyasagar Academy</h2>
            <p><em>Welcome to Vidyasagar Academy, where we strive for academic excellence and holistic development.</em></p>
            <h3>School Overview</h3>
            <p>Our school is a co-educational institution that provides a nurturing environment for students to grow and thrive.</p>
            <h3>Featured News and Events</h3>
            <ul>
                <li>Upcoming Science Fair: Register Now!</li>
                <li>New STEM Program Launched for Grades 9-10</li>
            </ul>
        </section>

        <!-- About Us -->
        <section id="about" class="tab-content">
            <h2>About Us</h2>
            <h3>School History</h3>
            <p>Founded in [Year], our school has a rich history of providing quality education to students from diverse backgrounds.</p>
            <h3>Mission and Vision</h3>
            <p>Our mission is to empower students with knowledge, skills, and values to succeed in an ever-changing world.</p>
            <h3>Administration and Staff</h3>
            <ul>
                <li>Meet Our Principal: [Name]</li>
                <li>Our Dedicated Faculty and Staff</li>
            </ul>
        </section>

        <!-- Academics -->
        <section id="academics" class="tab-content">
            <h2>Academics</h2>
            <h3>Curriculum</h3>
            <p>Our curriculum is designed to provide a balanced education that fosters intellectual, physical, and emotional growth.</p>
            <h3>Courses and Programs</h3>
            <ul>
                <li>STEM Programs</li>
                <li>Arts and Humanities</li>
            </ul>
            <h3>Faculty and Departments</h3>
            <ul>
                <li>Meet Our Faculty Members</li>
                <li>Department of Mathematics</li>
                <li>Department of Science</li>
            </ul>
        </section>

        <!-- Login -->
        <section id="login" class="tab-content">
            <h2>Login</h2>
            <h3>Student Login</h3>
            <p>Access your student portal to view grades, assignments, and more.</p>
            <h3>Teacher Login</h3>
            <p>Login to access teacher resources and gradebook.</p>
            <h3>Admin Login</h3>
            <p>Admin login for school administration and management.</p>
            <h3>Super Admin Login</h3>
            <p>Super admin login for system administration and configuration.</p>
            <h3>Parents Login</h3>
            <p>Parents login to access student information and progress reports.</p>
        </section>

        <!-- Admissions -->
        <section id="admissions" class="tab-content">
            <h2>Admissions</h2>
            <h3>Admission Process</h3>
            <p>Learn about our admission process and requirements.</p>
            <h3>Requirements and Deadlines</h3>
            <p>Admission Requirements and Deadlines</p>
            <h3>Tuition and Fees</h3>
            <p>Tuition Fees and Payment Options</p>
        </section>

        <!-- Student Life -->
        <section id="studentlife" class="tab-content">
            <h2>Student Life</h2>
            <h3>Extracurricular Activities</h3>
            <p>Join our clubs and activities to develop new skills and interests.</p>
            <h3>Clubs and Organizations</h3>
            <ul>
                <li>Debate Club</li>
                <li>Robotics Club</li>
            </ul>
            <h3>Student Council</h3>
            <p>Meet Our Student Council Members</p>
        </section>

        <!-- Resources -->
        <section id="resources" class="tab-content">
            <h2>Resources</h2>
            <h3>Library and Research</h3>
            <p>Access our library resources and research facilities.</p>
            <h3>Technology and IT</h3>
            <p>Learn about our technology infrastructure and IT support.</p>
            <h3>Support Services</h3>
            <p>Get support for counseling, academic advising, and more.</p>
        </section>

        <!-- News and Events -->
        <section id="news" class="tab-content">
            <h2>News and Events</h2>
            <h3>Latest News and Updates</h3>
            <p>Stay up-to-date with the latest news and updates from our school.</p>
            <h3>Upcoming Events and Calendar</h3>
            <p>View our upcoming events and calendar.</p>
        </section>

        <!-- Contact Us -->
        <section id="contact" class="tab-content">
            <h2>Contact Us</h2>
            <h3>Contact Information</h3>
            <p>Get in touch with us through phone, email, or mail.</p>
            <h3>Map and Directions</h3>
            <p>Find us on the map and get directions.</p>
            <h3>Online Inquiry Form</h3>
            <form id="inquiryForm" action="#" method="post" onsubmit="return handleFormSubmit(event)">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required />

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required />

                <label for="subject">Subject:</label>
                <input type="text" id="subject" name="subject" required />

                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="5" required></textarea>

                <button type="submit">Send Message</button>
            </form>
            <p id="formMessage" style="color: green; font-weight: bold; display:none; margin-top:1rem;"></p>
        </section>
    </main>
    <footer>
        &copy; 2024 Vidyasagar Academy. All rights reserved.
    </footer>

    <script>
        // Tab navigation
        const navLinks = document.querySelectorAll('.nav-link');
        const tabContents = document.querySelectorAll('.tab-content');

        navLinks.forEach(link => {
            link.addEventListener('click', e => {
                e.preventDefault();
                const target = link.getAttribute('data-tab');

                // Remove active from all
                navLinks.forEach(l => l.classList.remove('active'));
                tabContents.forEach(tc => tc.classList.remove('active'));

                // Add active to clicked
                link.classList.add('active');
                document.getElementById(target).classList.add('active');

                // Scroll to top of main content
                window.scrollTo({ top: 0, behavior: 'smooth' });
            });
        });

        // Set first nav link active on load
        navLinks[0].classList.add('active');

        // Simple form submission handler (mock)
        function handleFormSubmit(event) {
            event.preventDefault();
            const formMessage = document.getElementById('formMessage');
            formMessage.textContent = "Thank you for your inquiry. We will get back to you soon.";
            formMessage.style.display = 'block';
            event.target.reset();
            return false;
        }
    </script>
</body>
</html>
```# Vidyasagar-academy-
