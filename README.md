<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sidebar Menu</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="sidebar">
        <div class="header">Menu</div>
        <a href="#home" data-icon="🏠"><span>Home</span></a>
        <a href="#services" data-icon="💼"><span>Services</span></a>
        <a href="#about" data-icon="ℹ️"><span>About</span></a>
        <a href="#contact" data-icon="📞"><span>Contact</span></a>
    </div>
    <button class="toggle-btn" onclick="toggleSidebar()">☰</button>
    <main>
        <h1>Welcome to Our Website</h1>
        <p>Main content goes here...</p>
    </main>
    <script>
        function toggleSidebar() {
            document.querySelector('.sidebar').classList.toggle('collapsed');
            document.querySelector('.toggle-btn').classList.toggle('collapsed');
        }
    </script>
</body>
</html>
