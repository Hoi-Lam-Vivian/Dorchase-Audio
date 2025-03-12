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
