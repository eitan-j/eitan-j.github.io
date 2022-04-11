<!DOCTYPE html>
<html lang="en-US">
<head>
    <title>{{ page.title }}</title>
    <link rel="icon" type="image/x-icon" href="favicon.ico">
    <link rel="stylesheet" href="default.css">
</head>
<body>
    <header>
        <nav>
            <a {% if page.name == "index.md" %} class="currentpage" {% endif %} href="index.html">Home</a>
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