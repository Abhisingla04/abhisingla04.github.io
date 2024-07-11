---
layout: default
title: Home
permalink: /project/material-characterization/
---

<!-- Inline CSS for customization -->
<style>
  body {
      font-family: Arial, sans-serif;
      background-color: #FFFFFF;
      color: #333;
      margin: 0; /* Remove default margin */
      padding: 0; /* Remove default padding */
  }

  .content {
      margin: 20px auto; /* Center the content with auto margins */
      max-width: 800px; /* Set a maximum width for large screens */
      padding: 20px; /* Add padding around the content */
      background-color: #fff; /* Background color for the content area */
      box-shadow: 0 0 0px rgba(0, 0, 0, 0); /* Add a subtle shadow */
  }

  h1, h2, h3 {
      color: #0056b3;
      margin-top: 20px; /* Set top margin for headings */
  }

  p {
      margin-bottom: 15px; /* Set bottom margin for paragraphs */
  }

  a {
      color: #0056b3;
      text-decoration: none;
  }

  a:hover {
      text-decoration: underline;
  }

  /* Responsive design for smaller screens */
  @media (max-width: 600px) {
      .content {
          margin: 10px; /* Reduce margin for smaller screens */
          padding: 15px; /* Reduce padding for smaller screens */
      }

      h1, h2, h3 {
          margin-top: 15px; /* Reduce top margin for headings on smaller screens */
      }

      p {
          margin-bottom: 10px; /* Reduce bottom margin for paragraphs on smaller screens */
      }
  }
</style>


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Subpage 1</title>
    <link rel="stylesheet" type="text/css" href="/assets/css/styles.css">
</head>
<body>
    <div class="content" id="content"></div>

    <script>
        // Function to load content from an external file
        function loadContent() {
            fetch('content.html')
                .then(response => response.text())
                .then(data => {
                    document.getElementById('content').innerHTML = data;
                })
                .catch(error => console.error('Error loading content:', error));
        }

        // Load the content when the page loads
        window.onload = loadContent;
    </script>
</body>
</html>