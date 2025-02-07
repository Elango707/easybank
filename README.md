

/* Basic reset and global styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

/* Navbar styles */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #333;
    padding: 1rem 2rem;
    color: white;
}

.navbar .logo a {
    text-decoration: none;
    color: white;
    font-size: 1.5rem;
    font-weight: bold;
}

.navbar .nav-links ul {
    display: flex;
    list-style-type: none;
}

.navbar .nav-links li {
    margin-left: 20px;
}

.navbar .nav-links a {
    text-decoration: none;
    color: white;
    font-size: 1rem;
    transition: color 0.3s;
}

.navbar .nav-links a:hover,
.navbar .nav-links a:focus {
    color: #f0a500;
}

.menu-toggle {
    display: none;
    cursor: pointer;
}

.menu-toggle .bar {
    width: 25px;
    height: 3px;
    background-color: white;
    margin: 5px 0;
}

/* Hero section styles */
.hero {
    text-align: center;
    padding: 4rem 2rem;
    background-color: #1e2a47;
    color: white;
}

.hero h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.hero p {
    font-size: 1.25rem;
    margin-bottom: 2rem;
}

.cta-btn {
    background-color: #f0a500;
    color: white;
    padding: 0.75rem 2rem;
    font-size: 1rem;
    border: none;
    cursor: pointer;
    transition: background-color 0.3s;
}

.cta-btn:hover,
.cta-btn:focus {
    background-color: #d88b00;
}

/* Footer styles */
footer {
    text-align: center;
    padding: 1rem;
    background-color: #333;
    color: white;
}

/* Responsive styles */
@media (max-width: 768px) {
    .navbar .nav-links {
        display: none;
    }

    .navbar .menu-toggle {
        display: block;
    }

    .navbar .nav-links.active {
        display: block;
        position: absolute;
        top: 60px;
        right: 20px;
        background-color: #333;
        width: 200px;
        text-align: right;
        padding: 1rem;
    }

    .navbar .nav-links ul {
        flex-direction: column;
    }

    .navbar .nav-links li {
        margin: 10px 0;
    }
}
