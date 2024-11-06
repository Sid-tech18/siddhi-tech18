/* General Styles */
body {
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #282a3b;
}

/* Navigation Styles */
header {
    background-color: yellow;
    padding: 10px;
    position: sticky;
    top: 0;
    z-index: 1000;
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: space-around;
}

nav a {
    color: black;
    text-decoration: none;
    padding: 10px 15px;
}

nav a:hover {
    background-color: ;
}

/* Section Styles */
section {
    padding: 50px;
    margin: 20px;
    background-color: pink;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h1, h2 {
    color: #333;
}

/* Footer Styles */
footer {
    text-align: center;
    padding: 15px;
    background-color: #333;
    color: greenyellow;
    position: fixed;
    bottom: 0;
    width: 100%;
}



// Smooth scroll functionality for navigation links
document.querySelectorAll('nav a').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
            behavior: 'smooth'
        });
    });
});
