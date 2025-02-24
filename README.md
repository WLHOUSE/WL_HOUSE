# WL_HOUSE/* Global Styles */
body {
    font-family: 'Playfair Display', serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background-color: #f0f0f0;
    color: #333;
}

h1, h2, p {
    margin: 0;
}

a {
    text-decoration: none;
    color: inherit;
}

/* Section Hero */
.hero {
    position: relative;
    background-image: url('wwww.jpg');
    background-size: cover;
    background-position: center;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}

.overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.5);
}

.text-container {
    position: relative;
    color: #fff;
    text-align: center;
    padding: 20px;
}

.animated-text {
    opacity: 0;
    transform: translateY(30px);
    animation: fadeInUp 2s forwards;
}

.animated-text:nth-child(1) {
    animation-delay: 0.5s;
}

.animated-text:nth-child(2) {
    animation-delay: 1s;
}

@keyframes fadeInUp {
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Navigation */
nav {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: rgba(255, 255, 255, 0.8);
    padding: 10px;
    text-align: center;
}

nav ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    font-size: 18px;
    font-weight: bold;
    text-transform: uppercase;
    color: #333;
}

nav ul li a:hover {
    color: #856c58;
}

/* Section Robes */
#robes {
    padding: 50px 20px;
    text-align: center;
}

.robes-gallery {
    display: flex;
    justify-content: center;
    gap: 20px;
}

.robe-item img {
    width: 300px;
    height: 300px;
    object-fit: cover;
    border-radius: 10px;
    transition: transform 0.3s ease-in-out;
}

.robe-item p {
    margin-top: 10px;
    font-size: 16px;
}

.robe-item:hover img {
    transform: scale(1.05);
}

/* Section Contact */
#contact form {
    max-width: 600px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 10px;
}

#contact input, #contact textarea {
    padding: 10px;
    font-size: 16px;
    border-radius: 5px;
    border: 1px solid #ccc;
}

#contact button {
    padding: 10px;
    background-color: #f4a261;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

#contact button:hover {
    background-color: #e76f51;
}
