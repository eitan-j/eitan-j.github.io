<!DOCTYPE html>
<html lang="en-US">
<head>
    <title>{{ page.title }}</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="icon" type="image/x-icon" href="favicon.ico">
    <link rel="stylesheet" href="default.css">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans&family=Noto+Sans+Hebrew&display=swap" rel="stylesheet"> 
</head>
<body>
    <header>
        <nav>
            <a {% if page.name == "index.md" %} class="currentpage" {% endif %} href="/">Home</a>
            <a {% if page.name == "resume.md" %} class="currentpage" {% endif %} href="resume.html">Resume</a>
            <!-- <a {% if page.name == "writing.md" %} class="currentpage" {% endif %} href="writing.html">Writing</a> -->
            <a {% if page.name == "about.md" %} class="currentpage" {% endif %} href="about.html">About</a>
        </nav>
    </header>
    <main>
    {{ content }}
    </main>
</body>
</html>