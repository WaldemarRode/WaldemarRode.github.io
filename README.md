# Portfolio Website Documentation

## Overview

This documentation provides an overview of the portfolio website project for a third-year IT student. The website is designed to showcase the student's skills, projects, and resume. The project consists of multiple pages: Home, About, Projects, Contact, and a link to the Resume/CV. The website is built using HTML, CSS, and includes an external CSS file for styling.

## Table of Contents

1. [Project Structure](#project-structure)
2. [Pages Description](#pages-description)
3. [CSS Styling](#css-styling)
4. [Images](#images)
5. [Resume/CV](#resumecv)
6. [Setup and Deployment](#setup-and-deployment)

## Project Structure

The project directory contains the following files:

```
/portfolio-website
|-- index.html
|-- aboutme.html
|-- projects.html
|-- contact.html
|-- CV.pdf
|-- mystyle.css
|-- githublogooo.jpg
```

### File Descriptions

- **index.html**: The homepage of the portfolio website.
- **aboutme.html**: The About page with information about the student.
- **projects.html**: The Projects page showcasing the student's projects.
- **contact.html**: The Contact page with contact details.
- **CV.pdf**: The student's resume/CV.
- **mystyle.css**: The external CSS file for styling the website.
- **githublogooo.jpg**: Images used in the Projects page.

## Pages Description

### index.html

The homepage introduces the portfolio website. It contains a navigation bar with links to the other pages and a brief welcome message.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Waldemar Rode</title>
    <link rel="stylesheet" href="mystyle.css">
</head>
<body>
    <div class="navbar">
        <div class="left">
            <a href="./">Home</a>
        </div>
        <div class="right">
            <a href="./aboutme">About</a>
            <a href="./projects">Projects</a>
            <a href="./contact">Contact</a>
            <a href="CV.pdf" target="_blank">Resume/CV</a>
        </div>
    </div>
    <div class="content">
        <div class="container">
            <div class="heading">
                <h1>Welcome to My Portfolio</h1>
                <p>I am Waldemar Rode, a 3rd year student at North-West University</p>
            </div>
        </div>
    </div>
</body>
</html>
```

### aboutme.html

The About page provides a brief description of the student, their background, and their interests.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About - Waldemar Rode</title>
    <link rel="stylesheet" href="mystyle.css">
</head>
<body>
    <div class="navbar">
        <div class="left">
            <a href="./">Home</a>
        </div>
        <div class="right">
            <a href="./aboutme">About</a>
            <a href="./projects">Projects</a>
            <a href="./contact">Contact</a>
            <a href="CV.pdf" target="_blank">Resume/CV</a>
        </div>
    </div>
    <div class="content">
        <div class="container">
            <div class="section">
                <h2>About Me</h2>
                <p>I am a final year Information Technology student at North West University. I have a passion for coding, web development, and creating innovative solutions to complex problems. This portfolio showcases some of my projects and accomplishments throughout my academic journey.</p>
            </div>
        </div>
    </div>
</body>
</html>
```

### projects.html

The Projects page lists the student's projects, each with a brief description and an image.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projects - Waldemar Rode</title>
    <link rel="stylesheet" href="mystyle.css">
</head>
<body>
    <div class="navbar">
        <div class="left">
            <a href="./">Home</a>
        </div>
        <div class="right">
            <a href="./aboutme">About</a>
            <a href="./projects">Projects</a>
            <a href="./contact">Contact</a>
            <a href="CV.pdf" target="_blank">Resume/CV</a>
        </div>
    </div>
    <div class="content">
        <div class="container">
            <div class="section">
                <h2>My Projects</h2>
                <div class="project-item">
                    <p><strong>Project 1:</strong>This Portfolio Website.</p>
                    <a href="https://github.com/WaldemarRode/WaldemarRode.github.io">
                        <img src="githublogooo.jpg" alt="Project 1 Image">
                    </a>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
```

### contact.html

The Contact page provides the student's contact information and links to their LinkedIn profile.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact - Waldemar Rode</title>
    <link rel="stylesheet" href="mystyle.css">
</head>
<body>
    <div class="navbar">
        <div class="left">
            <a href="./">Home</a>
        </div>
        <div class="right">
            <a href="./aboutme">About</a>
            <a href="./projects">Projects</a>
            <a href="./contact">Contact</a>
            <a href="CV.pdf" target="_blank">Resume/CV</a>
        </div>
    </div>
    <div class="content">
        <div class="container">
            <div class="section">
                <h2>Contact Me</h2>
                <p>If you would like to get in touch, please feel free to reach out via email or connect with me on LinkedIn.</p>
                <p>Email: <a href="mailto:rodewaldemar2@gmail.com">rodewaldemar2@gmail.com</a></p>
                <p>LinkedIn: <a href="www.linkedin.com/in/waldemar-rode-49a7b8272" target="_blank">www.linkedin.com/in/waldemar-rode-49a7b8272</a></p>
            </div>
        </div>
    </div>
</body>
</html>
```

## CSS Styling

The `styles.css` file contains the styling for the website. It uses Flexbox for layout and ensures that the navigation bar is responsive and links are appropriately aligned.

```css
/* styles.css */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

.navbar {
    display: flex;
    justify-content: space-between;
    background-color: rgba(51, 51, 51, 0.9);
    padding: 0 20px;
}

.navbar .left {
    display: flex;
}

.navbar .right {
    display: flex;
}

.navbar a {
    display: block;
    color: white;
    text-align: center;
    padding: 14px 20px;
    text-decoration: none;
}

.navbar a:hover {
    background-color: #ddd;
    color: black;
}

.content {
    flex: 1;
    display: flex;
    align-items: center;
    justify-content: center;
}

.container {
    max-width: 800px;
    padding: 20px;
    background-color: rgba(255, 255, 255, 0.9);
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    border-radius: 10px;
}

.heading, .section {
    text-align: center;
    margin-bottom: 40px;
}

.section h2 {
    color: #333;
}

.section p {
    text-align: justify;
    color: #666;
}

.project-item

 {
    margin-bottom: 30px;
}

.project-item img {
    width: 100%;
    max-width: 400px;
    display: block;
    margin: 10px auto;
}
```

## Images

Replace placeholder image (`githublogooo.jpg`) with your own project image. Ensure the image is optimized for web usage.

## Resume/CV

Place your `CV.pdf` file in the root directory of your project. The link in the navigation bar will open this file in a new tab.

## Setup and Deployment

1. **Setup**: Ensure all files are in the same directory structure as described in the Project Structure section.
2. **Local Testing**: Open each HTML file in your web browser to test the website locally.
3. **Deployment**: Upload the entire project directory to a web server or hosting service. Ensure all file paths are correctly referenced and the resume file is accessible.

### Additional Notes

- Keep the CSS modular and well-commented for future maintenance.
- Consider adding more interactivity using JavaScript for a more dynamic user experience.
- Test the website across different browsers and devices to ensure responsiveness and compatibility.

This documentation should provide a comprehensive guide for setting up and understanding the structure and functionality of the portfolio website.