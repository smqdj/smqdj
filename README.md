<!-- Add this code to the "theme.liquid" file in your Shopify theme editor -->

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>{{ shop.name }}</title>
  {{ content_for_header }}
  <style>
    /* Customize your styles here */
    body {
      font-family: 'Arial', sans-serif;
      background-color: #f7f7f7;
      color: #333;
    }
    header {
      background-color: #fff;
      padding: 20px;
      border-bottom: 1px solid #eee;
      text-align: center;
    }
    h1, h2, h3 {
      color: #555;
    }
    .main-content {
      padding: 20px;
    }
    footer {
      background-color: #333;
      color: #fff;
      padding: 10px;
      text-align: center;
    }
  </style>
</head>
<body>
  <header>
    <h1>{{ shop.name }}</h1>
    <p>Your tagline here</p>
  </header>

  <div class="main-content">
    {{ content_for_layout }}
  </div>

  <footer>
    <p>&copy; {{ 'now' | date: '%Y' }} {{ shop.name }}. All rights reserved.</p>
  </footer>
</body>
</html>
