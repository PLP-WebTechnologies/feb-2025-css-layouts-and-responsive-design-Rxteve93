# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨


HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trapid Hub</title>
    <link rel="stylesheet" href="css layout.css">
</head>
<body>
    
    <header>
        <nav class="navbar">
            <div class="logo">Trapid Hub</div>
            <ul class="nav-links">
        
                <li><a href="#">Home</a></li>
                <li><a href="https://www.instagram.com/trapid_hub/?next=%2F">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="https://wa.link/ydja5x">Contact</a></li>
            </ul>
            
        </nav>
    </header>

    <main class="container">
        <section class="hero">
            <h1>Welcome to Trapid Hub</h1>
            <p>Re-defining People and Business Development</p>
            
        </section>
<p>
    <h2>
        What are digital skills?
    </h2> </p>
    <p>
            Digital skills are the abilities needed to use digital devices, software, and the internet effectively. They range from basic computer literacy, such as using email and browsing the web, to advanced skills like coding, data analysis, cybersecurity, and digital marketing. These skills are essential for work, communication, and innovation in today's technology-driven world. 
    </p>
    <p>
        Trapid Hub offers several courses,with robust resources, that provide learners with extensive knowledge on the trending skillsets needed to successfully thrive in the digital space. <p>These digital skills are listed below;</p>
    </p>

        <section class="grid-layout"class="grid-layout">
           <div class="card">Web Development</div>
            <div class="card">Digital Marketing</div>
            <div class="card">Data Analytics</div>
            <div class="card">Cybersecurity</div>
            <div class="card">Product Design</div>
            <div class="card">Social Media Management</div>
        </section>
    </main>
    <h4><strong>Join the next generation of techstars!!!</strong> </h4>
    <p>
    <button class="btn">Get Started</button>
    </p>
    <footer>
        <p>&copy; 2025 Trapid Hub. All rights reserved.</p>
    </footer>
</body>

</html>


CSS

/* General Styles */
body {
    font-family: Arial, sans-serif;
    margin: 20px;
    padding: 20px;
    box-sizing: border-box;
    background-color: #f8f8f8;
}

/* Navigation Bar */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #f5f4f4;
    color: rgba(22, 228, 8, 0.621);
    padding: 15px 20px;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 20px;
}

.nav-links li {
    display: inline;
}

.nav-links a {
    text-decoration: none;
    color: rgb(1, 1, 1);
}

/* Hero Section */
.hero {
    text-align: center;
    padding: 50px 20px;
    background: rgba(2, 225, 77, 0.568);
    color: white;
}

.btn {
    padding: 10px 20px;
    background: hsla(140, 95%, 46%, 0.797);
    color: #040505;
    border: none;
    cursor: pointer;
    border-radius: 8px;
    align-items: center;
}

/* Grid Layout */
.grid-layout {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
    padding: 20px;
}

.card {
    background: white;
    padding: 20px;
    text-align: center;
    border-radius: 8px;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
}

/* Footer */
footer {
    text-align: center;
    background: #333;
    color: white;
    padding: 10px;
}

/* Responsive Design */
@media (max-width: 768px) {
    .grid-layout {
        grid-template-columns: 1fr;
    }

    .nav-links {
        display: none;
    }
    
    section {
        padding: 20px;
    }
