# Task4
Mobile-Friendly Website using CSS Media Queries

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Page</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <nav>
      <ul class="nav">
        <li>Home</li>
        <li>About</li>
        <li>Contact</li>
      </ul>
    </nav>
  </header>
  <main class="content">
    <div class="column left">Left column</div>
    <div class="column right">Right column</div>
  </main>
</body>
</html>
/* Base styles for desktop */
.nav {
  display: flex;
  gap: 20px;
}

.content {
  display: flex;
  gap: 20px;
}

.column {
  width: 50%;
}

img {
  max-width: 100%;
  height: auto;
}

/* Mobile adjustments */
@media (max-width: 768px) {
  .nav {
    flex-direction: column;
    align-items: flex-start;
  }

  .content {
    flex-direction: column;
  }

  .column {
    width: 100%;
    padding: 10px;
  }

  body {
    font-size: 14px;
  }
}
