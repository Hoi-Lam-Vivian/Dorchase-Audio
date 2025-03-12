<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dorchase Audio - Home</title>
    <link href="https://example.com/path/to/STLiti.ttf" rel="stylesheet" type="font/ttf">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        @font-face {
            font-family: 'STLiti';
            src: url('your-path/STLiti.ttf') format('truetype');
        }
        body {
            font-family: "Baloo Bhai 2", Arial, sans-serif;
            background: #151f29;
            min-height: 100vh;
            display: flex; /* 使用 Flexbox */
        }

        :root {
            --menu-width: 300px;
            --collapsed-width: 60px;
        }

        aside {
            padding: 10px;
            position: fixed;
            min-height: 100vh;
            background: linear-gradient(0deg, black, #1f314b);
            width: 300px;
            color: white;
            transition: .3s;
            box-shadow: 0px 0px 15px 0px #00000073;
            z-index: 1;
        }

        .collapsed aside {
            width: var(--collapsed-width);
        }

        .menu-btn {
            color: white;
            position: absolute;
            top: 20px;
            right: 0;
            padding: 8px;
            border: none;
            font-size: 15px;
            aspect-ratio: 1;
            border-radius: 0 50% 50% 0;
            cursor: pointer;
            transform: translateX(100%);
            box-shadow: 2px 0px 5px 0px #1a1a1a;
            background: #1b2b42;
        }

        .logo-wrapper {
            display: flex;
            overflow: hidden;
            white-space: nowrap;
            align-items: center;
            gap: 15px;
            padding: 10px;
        }

        a {
            text-decoration: none;
            color: white;
        }

        .fa-uikit:before {
            font-size: 25px;
        }

        .brand-name {
            font-size: 20px;
            transition: .3s;
        }

        .collapsed .brand-name {
            width: 0;
            visibility: hidden;
            transition-delay: .3s;
        }

        .separator {
            width: 100%;
            height: 1px;
            background-color: rgb(171 171 171 / 21%);
        }

        .menu-items {
            margin-top: 15px;
        }

        ul {
            list-style: none;
        }

        .menu-items a {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 10px;
            margin-bottom: 10px;
            overflow: hidden;
        }

        .menu-items a:hover {
            color: #daddff;
            background: #00000017;
            border-radius: 10px;
        }

        .menu-items li {
            position: relative;
        }

        .icon {
            font-size: 20px;
        }

        .item-name {
            transition: .3s;
        }

        .collapsed .item-name {
            width: 0;
            visibility: hidden;
            transition-delay: .3s;
        }

        .tooltip {
            position: absolute;
            right: -25px;
            top: 50%;
            color: white;
            padding: 5px 15px;
            font-size: 15px;
            line-height: 1.5;
            border-radius: 5px;
            opacity: 0;
            visibility: hidden;
            transition: opacity .3s;
            background-color: rgb(22, 22, 22);
            transform: translate(100%, -50%);
        }

        .collapsed .menu-items a:hover+.tooltip {
            visibility: visible;
            opacity: 1;
        }

        .tooltip::before {
            content: "\f0d9";
            font-family: 'Font Awesome 6 Free';
            position: absolute;
            font-weight: 900;
            left: 0;
            top: 50%;
            font-size: 30px;
            color: #161616;
            transform: translate(-50%, -50%);
        }

        main {
            position: relative;
            left: calc(var(--menu-width) + 20px);
            width: calc(100% - (var(--menu-width) + 20px));
            transition: .3s;
            padding: 10px;
            color: white;
        }

        .collapsed main {
            left: calc(var(--collapsed-width) + 20px);
        }
    </style>
</head>
<body>

<header>
    <h1>Dorchase Audio</h1>
    <nav>
        <a href="index.html">Home</a>
        <a href="products.html">Products</a>
        <a href="about.html">About Us</a>
        <a href="support.html">Support</a>
    </nav>
</header>

<aside>
    <button class="menu-btn fa fa-chevron-left"></button>
    <a href="/" class="logo-wrapper">
        <span class="fa-brands fa-uikit"></span>
        <span class="brand-name">Dorchase Audio</span> 
    </a>
    <div class="separator"></div>
    <ul class="menu-items">
        <li><a href="index.html"><span class="icon fa fa-house"></span><span class="item-name">Home</span></a><span class="tooltip">Home</span></li>
        <li><a href="products.html"><span class="icon fa fa-box"></span><span class="item-name">Products</span></a><span class="tooltip">Products</span></li>
        <li><a href="about.html"><span class="icon fa fa-info-circle"></span><span class="item-name">About</span></a><span class="tooltip">About Us</span></li>
        <li><a href="support.html"><span class="icon fa fa-comment-dots"></span><span class="item-name">Contact Us</span></a><span class="tooltip">Contact Us</span></li>
    </ul>
</aside>

<main>
    <div class="container">
        <div class="hero">
            <h1>Enjoy the Art of Music</h1>
            <p>Explore our audio products and enhance your listening experience.</p>
            <a href="products.html">View Products</a>
        </div>

        <section class="features">
            <div class="feature">
                <h2>High-Quality Audio</h2>
                <p>We offer a variety of high-quality audio equipment designed to enhance your listening experience.</p>
            </div>
            <div class="feature">
                <h2>Professional Design</h2>
                <p>Each product is meticulously designed to combine aesthetics and functionality.</p>
            </div>
            <div class="feature">
                <h2>Customer Support</h2>
                <p>Our customer support team is always here to answer your questions and provide assistance.</p>
            </div>
        </section>
    </div>
</main>

<footer>
    <p>Contact Us | Privacy Policy | Terms of Use</p>
    <p>&copy; 2025 Dorchase Audio. All rights reserved.</p>
</footer>

</body>
</html>

<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dorchase Audio - Products</title>
    <link href="https://example.com/path/to/STLiti.ttf" rel="stylesheet" type="font/ttf">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {
            --menu-width: 300px;
            --collapsed-width: 60px;
            --background-color: #151f29;
            --text-color: white;
            --hover-color: #daddff;
            --link-color: white;
        }

        body {
            font-family: "Baloo Bhai 2", Arial, sans-serif;
            background: var(--background-color);
            color: var(--text-color);
            min-height: 100vh;
            display: flex;
        }

        header, footer {
            padding: 10px;
            background-color: #1b2b42;
            text-align: center;
        }

        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: var(--link-color);
        }

        aside {
            padding: 10px;
            position: fixed;
            min-height: 100vh;
            background: linear-gradient(0deg, black, #1f314b);
            width: var(--menu-width);
            color: var(--text-color);
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.3);
        }

        .menu-btn {
            color: var(--text-color);
            position: absolute;
            top: 20px;
            right: 0;
            padding: 8px;
            border: none;
            background: #1b2b42;
            cursor: pointer;
        }

        .logo-wrapper {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 10px;
        }

        .menu-items {
            margin-top: 15px;
            list-style: none;
            padding: 0;
        }

        .menu-items a {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 10px;
            margin-bottom: 10px;
            color: var(--text-color);
            transition: background 0.3s;
        }

        .menu-items a:hover {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 5px;
        }

        main {
            margin-left: calc(var(--menu-width) + 20px);
            width: calc(100% - (var(--menu-width) + 20px));
            padding: 10px;
        }

        footer {
            margin-top: auto; /* Push footer to the bottom */
        }
    </style>
</head>
<body>

<header>
    <h1>Dorchase Audio</h1>
    <nav>
        <a href="index.html">Home</a>
        <a href="products.html">Products</a>
        <a href="about.html">About Us</a>
        <a href="support.html">Support</a>
    </nav>
</header>

<aside>
    <button class="menu-btn fa fa-chevron-left" aria-label="Toggle menu"></button>
    <a href="/" class="logo-wrapper">
        <span class="fa-brands fa-uikit"></span>
        <span class="brand-name">Dorchase Audio</span>
    </a>
    <div class="separator"></div>
    <ul class="menu-items">
        <li><a href="index.html"><span class="icon fa fa-house"></span><span class="item-name">Home</span></a></li>
        <li><a href="products.html"><span class="icon fa fa-box"></span><span class="item-name">Products</span></a></li>
        <li><a href="about.html"><span class="icon fa fa-info-circle"></span><span class="item-name">About</span></a></li>
        <li><a href="support.html"><span class="icon fa fa-comment-dots"></span><span class="item-name">Contact Us</span></a></li>
    </ul>
</aside>

<main>
    <h2>Our Products</h2>
    <p>我們提供多種高品質的音響產品，包括：</p>
    <ul>
        <li>Dorchase DBS512ProA - 五吋書架箱喇叭</li>
        <li>Dorchase DA805 - Hybird Integrated Amplifier</li>
        <li>Dorchase DSW6.0 - 6 inch Spheric Passive Subwoofer with two passive radiators</li>
    </ul>
</main>

<footer>
    <p>聯繫我們 | 隱私政策 | 使用條款</p>
    <p>&copy; 2025 Dorchase Audio. 版權所有</p>
</footer>

</body>
</html>

<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dorchase Audio - Abouts</title>
    <link href="https://example.com/path/to/STLiti.ttf" rel="stylesheet" type="font/ttf">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {
            --menu-width: 300px;
            --collapsed-width: 60px;
            --background-color: #151f29;
            --text-color: white;
            --hover-color: #daddff;
            --link-color: white;
        }

        body {
            font-family: "Baloo Bhai 2", Arial, sans-serif;
            background: var(--background-color);
            color: var(--text-color);
            min-height: 100vh;
            display: flex;
        }

        header, footer {
            padding: 10px;
            background-color: #1b2b42;
            text-align: center;
        }

        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: var(--link-color);
        }

        aside {
            padding: 10px;
            position: fixed;
            min-height: 100vh;
            background: linear-gradient(0deg, black, #1f314b);
            width: var(--menu-width);
            color: var(--text-color);
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.3);
        }

        .menu-btn {
            color: var(--text-color);
            position: absolute;
            top: 20px;
            right: 0;
            padding: 8px;
            border: none;
            background: #1b2b42;
            cursor: pointer;
        }

        .logo-wrapper {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 10px;
        }

        .menu-items {
            margin-top: 15px;
            list-style: none;
            padding: 0;
        }

        .menu-items a {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 10px;
            margin-bottom: 10px;
            color: var(--text-color);
            transition: background 0.3s;
        }

        .menu-items a:hover {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 5px;
        }

        main {
            margin-left: calc(var(--menu-width) + 20px);
            width: calc(100% - (var(--menu-width) + 20px));
            padding: 10px;
        }

        footer {
            margin-top: auto; /* Push footer to the bottom */
        }
    </style>
</head>
<body>

<header>
    <h1>Dorchase Audio</h1>
    <nav>
        <a href="index.html">Home</a>
        <a href="products.html">Products</a>
        <a href="about.html">About Us</a>
        <a href="support.html">Support</a>
    </nav>
</header>

<aside>
    <button class="menu-btn fa fa-chevron-left" aria-label="Toggle menu"></button>
    <a href="/" class="logo-wrapper">
        <span class="fa-brands fa-uikit"></span>
        <span class="brand-name">Dorchase Audio</span>
    </a>
    <div class="separator"></div>
    <ul class="menu-items">
        <li><a href="index.html"><span class="icon fa fa-house"></span><span class="item-name">Home</span></a></li>
        <li><a href="products.html"><span class="icon fa fa-box"></span><span class="item-name">Products</span></a></li>
        <li><a href="about.html"><span class="icon fa fa-info-circle"></span><span class="item-name">About</span></a></li>
        <li><a href="support.html"><span class="icon fa fa-comment-dots"></span><span class="item-name">Contact Us</span></a></li>
    </ul>
</aside>

<main>
    <h2>Our Story</h2>
    <p>Founded in 2020, Dorchase Audio is committed to providing the highest quality audio equipment to give music lovers the best sound experience.</p>
    <p>Our mission is to bring the beauty of music to every user.</p>
</main>

<footer>
    <p>聯繫我們 | 隱私政策 | 使用條款</p>
    <p>&copy; 2025 Dorchase Audio. 版權所有</p>
</footer>

</body>
</html>

<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dorchase Audio - Abouts</title>
    <link href="https://example.com/path/to/STLiti.ttf" rel="stylesheet" type="font/ttf">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {
            --menu-width: 300px;
            --collapsed-width: 60px;
            --background-color: #151f29;
            --text-color: white;
            --hover-color: #daddff;
            --link-color: white;
        }

        body {
            font-family: "Baloo Bhai 2", Arial, sans-serif;
            background: var(--background-color);
            color: var(--text-color);
            min-height: 100vh;
            display: flex;
        }

        header, footer {
            padding: 10px;
            background-color: #1b2b42;
            text-align: center;
        }

        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: var(--link-color);
        }

        aside {
            padding: 10px;
            position: fixed;
            min-height: 100vh;
            background: linear-gradient(0deg, black, #1f314b);
            width: var(--menu-width);
            color: var(--text-color);
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.3);
        }

        .menu-btn {
            color: var(--text-color);
            position: absolute;
            top: 20px;
            right: 0;
            padding: 8px;
            border: none;
            background: #1b2b42;
            cursor: pointer;
        }

        .logo-wrapper {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 10px;
        }

        .menu-items {
            margin-top: 15px;
            list-style: none;
            padding: 0;
        }

        .menu-items a {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 10px;
            margin-bottom: 10px;
            color: var(--text-color);
            transition: background 0.3s;
        }

        .menu-items a:hover {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 5px;
        }

        main {
            margin-left: calc(var(--menu-width) + 20px);
            width: calc(100% - (var(--menu-width) + 20px));
            padding: 10px;
        }

        footer {
            margin-top: auto; /* Push footer to the bottom */
        }
    </style>
</head>
<body>

<header>
    <h1>Dorchase Audio</h1>
    <nav>
        <a href="index.html">Home</a>
        <a href="products.html">Products</a>
        <a href="about.html">About Us</a>
        <a href="support.html">Support</a>
    </nav>
</header>

<aside>
    <button class="menu-btn fa fa-chevron-left" aria-label="Toggle menu"></button>
    <a href="/" class="logo-wrapper">
        <span class="fa-brands fa-uikit"></span>
        <span class="brand-name">Dorchase Audio</span>
    </a>
    <div class="separator"></div>
    <ul class="menu-items">
        <li><a href="index.html"><span class="icon fa fa-house"></span><span class="item-name">Home</span></a></li>
        <li><a href="products.html"><span class="icon fa fa-box"></span><span class="item-name">Products</span></a></li>
        <li><a href="about.html"><span class="icon fa fa-info-circle"></span><span class="item-name">About</span></a></li>
        <li><a href="support.html"><span class="icon fa fa-comment-dots"></span><span class="item-name">Contact Us</span></a></li>
    </ul>
</aside>

<main>
    <h2>需要幫助？</h2>
    <p>如果您在使用我們的產品時遇到任何問題，請隨時聯繫我們的客戶支持團隊。</p>
    <p>您可以發送電子郵件到 support@dorchaseaudio.com 或致電我們的客服熱線。</p>
</main>

<footer>
    <p>聯繫我們 | 隱私政策 | 使用條款</p>
    <p>&copy; 2025 Dorchase Audio. 版權所有</p>
</footer>

</body>
</html>
