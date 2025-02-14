- 👋 Hi, I’m @Naidurahul2001
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Naidurahul2001/Naidurahul2001 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dropdown Navigation Menu</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav>
        <ul class="main-nav">
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li class="dropdown">
                <a href="#">Services</a>
                <ul class="dropdown-menu">
                    <li><a href="#">Web Design</a></li>
                    <li><a href="#">SEO Services</a></li>
                    <li><a href="#">Digital Marketing</a></li>
                </ul>
            </li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>
</body>
</html>
/* Basic Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Styling the Navigation Bar */
nav {
    background-color: #333;
    padding: 10px 20px;
}

.main-nav {
    list-style-type: none;
    display: flex;
    justify-content: center;
    align-items: center;
}

.main-nav li {
    margin: 0 20px;
}

.main-nav a {
    text-decoration: none;
    color: #fff;
    font-size: 16px;
    padding: 10px;
    display: inline-block;
}

/* Dropdown Menu */
.dropdown {
    position: relative;
}

.dropdown-menu {
    display: none;
    position: absolute;
    background-color: #444;
    top: 100%;
    left: 0;
    min-width: 200px;
    border: 1px solid #333;
    list-style-type: none;
    padding: 10px 0;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
}

.dropdown-menu li {
    padding: 10px 20px;
}

.dropdown-menu li a {
    color: #fff;
    display: block;
}

/* Hover Effects */
.main-nav li:hover > a,
.dropdown-menu li:hover a {
    background-color: #555;
}

.dropdown:hover .dropdown-menu {
    display: block;
    animation: fadeIn 0.3s ease-in-out;
}

/* Optional Animation */
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(-10px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
