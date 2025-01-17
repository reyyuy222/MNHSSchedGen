<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Class Schedule Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 15px;
            text-align: center;
        }
        nav {
            text-align: center;
            margin: 20px 0;
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #333;
            font-size: 18px;
        }
        nav a:hover {
            color: #4CAF50;
        }
        .container {
            padding: 20px;
            text-align: center;
        }
        #schedule-form {
            display: none;
        }
        #schedule-form input, #schedule-form button {
            padding: 10px;
            margin: 10px;
        }
        #schedule-form button {
            background-color: #4CAF50;
            color: white;
            border: none;
        }
        footer {
            background-color: #4CAF50;
            color: white;
            padding: 10px;
            text-align: center;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Class Schedule Generator</h1>
    </header>
    <nav>
        <a href="#" id="home-link">Home</a>
        <a href="#" id="schedule-link">Class Schedule Generator</a>
    </nav>
    <div class="container" id="home-content">
        <h2>Home</h2>
        <p>This is the homepage of the Class Schedule Generator. Click the 'Class Schedule Generator' tab to create your custom schedule.</p>
    </div>
    <div class="container" id="schedule-form">
        <h2>Class Schedule Generator</h2>
        <form>
            <input type="text" placeholder="Enter Class Name" required>
            <input type="time" placeholder="Start Time" required>
            <input type="time" placeholder="End Time" required>
            <button type="submit">Generate Schedule</button>
        </form>
    </div>
    <footer>
        <p>&copy; 2025 Class Schedule Generator</p>
    </footer>
    <script>
        document.getElementById('schedule-link').addEventListener('click', function() {
            document.getElementById('home-content').style.display = 'none';
            document.getElementById('schedule-form').style.display = 'block';
        });
        document.getElementById('home-link').addEventListener('click', function() {
            document.getElementById('home-content').style.display = 'block';
            document.getElementById('schedule-form').style.display = 'none';
        });
    </script>
</body>
</html>
