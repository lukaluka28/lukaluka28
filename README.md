- 👋 Hi, I’m @lukaluka28
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
lukaluka28/lukaluka28 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Georgian Films</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Header Section -->
    <header>
        <h1>Georgian Films</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#films">Films</a></li>
                <li><a href="#reviews">Reviews</a></li>
                <li><a href="#news">News</a></li>
            </ul>
        </nav>
    </header>

    <!-- Featured Films Section -->
    <section id="home">
        <h2>Featured Georgian Films</h2>
        <div class="film-card">
            <h3>Film Title 1</h3>
            <p>Brief description of the film...</p>
        </div>
        <div class="film-card">
            <h3>Film Title 2</h3>
            <p>Brief description of the film...</p>
        </div>
    </section>

    <!-- Films Section -->
    <section id="films">
        <h2>All Films</h2>
        <div class="film-list">
            <div class="film-card">
                <h3>Film 1</h3>
                <p>Short summary of the film.</p>
            </div>
            <div class="film-card">
                <h3>Film 2</h3>
                <p>Short summary of the film.</p>
            </div>
            <div class="film-card">
                <h3>Film 3</h3>
                <p>Short summary of the film.</p>
            </div>
        </div>
    </section>

    <!-- Reviews Section -->
    <section id="reviews">
        <h2>Film Reviews</h2>
        <div class="review-card">
            <h3>Review of Film Title 1</h3>
            <p>Review content goes here...</p>
        </div>
    </section>

    <!-- News Section -->
    <section id="news">
        <h2>Film Industry News</h2>
        <div class="news-item">
            <h3>Latest News Headline</h3>
            <p>Details about the news...</p>
        </div>
    </section>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2024 Georgian Films. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
/* General Styles */
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: white;
    padding: 1em;
    text-align: center;
}

header h1 {
    margin: 0;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin-right: 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

section {
    padding: 20px;
    background-color: white;
    margin: 20px;
}

.film-card, .review-card, .news-item {
    background-color: #e1e1e1;
    padding: 15px;
    margin-bottom: 15px;
    border-radius: 8px;
}

.film-card h3, .review-card h3, .news-item h3 {
    margin-top: 0;
}

/* Footer Section */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 1em;
    position: fixed;
    width: 100%;
    bottom: 0;
}
// Simple script for expanding/collapsing film details when clicked
document.querySelectorAll('.film-card').forEach(card => {
    card.addEventListener('click', function() {
        this.classList.toggle('expanded');
    });
});
