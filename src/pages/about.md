/*
---
layout: ../layouts/AboutLayout.astro
title: "Submit"
---

AstroPaper is a minimal, responsive and SEO-friendly Astro blog theme. I designed and crafted this based on [my personal blog](https://satnaing.dev/blog).

This theme is aimed to be accessible out of the box. Light and dark mode are supported by
default and additional color schemes can also be configured.

This theme is self-documented \_ which means articles/posts in this theme can also be considered as documentations. So, see the documentation for more info.

<div>
  <img src="/assets/dev.svg" class="sm:w-1/2 mx-auto" alt="coding dev illustration">
</div>

## Tech Stack

This theme is written in vanilla JavaScript (+ TypeScript for type checking) and a little bit of ReactJS for some interactions. TailwindCSS is used for styling; and Markdown is used for blog contents.

## Features

Here are certain features of this site.

- fully responsive and accessible
- SEO-friendly
- light & dark mode
- fuzzy search
- super fast performance
- draft posts
- pagination
- sitemap & rss feed
- highly customizable

If you like this theme, you can star/contribute to the [repo](https://github.com/satnaing/astro-paper).  
Or you can even give any feedback via my [email](mailto:contact@satnaing.dev).
*/
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Email Submission</title>
    <style>
        .container {
            max-width: 400px;
            margin: 0 auto;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .input-group {
            margin-bottom: 20px;
        }
        .input-group label {
            display: block;
            margin-bottom: 5px;
        }
        .input-group input {
            width: 100%;
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 3px;
        }
        .btn-submit {
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 3px;
            padding: 10px 20px;
            cursor: pointer;
        }
        .btn-submit:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Email Submission</h2>
        <form id="emailForm">
            <div class="input-group">
                <label for="email">Email Address:</label>
                <input type="email" id="email" name="email" required>
            </div>
            <button type="submit" class="btn-submit">Submit</button>
        </form>
    </div>
    <script>
        document.getElementById("emailForm").addEventListener("submit", function(event) {
            event.preventDefault();
            const email = document.getElementById("email").value;
            // 在此处添加将电子邮件地址提交到后端的逻辑
            console.log("Email submitted:", email);
            // 清空表单字段
            document.getElementById("email").value = "";
        });
    </script>
</body>
</html>
