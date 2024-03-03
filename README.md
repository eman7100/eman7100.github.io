<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sample Academic Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Courses</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section>
            <h1>Welcome to Our Academic Website</h1>
            <p>This is a sample paragraph. Replace this with your own content to build out your website.</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Sample Academic Website</p>
    </footer>
</body>
</html>

/* Basic Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
}

header {
    background-color: #005A9C; /* Adjust the color to match AOU's theme */
    color: white;
    padding: 20px 0;
}

nav ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

main {
    padding: 20px;
    text-align: center;
}

footer {
    background-color: #003366; /* Adjust the color to match AOU's theme */
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Chatbot Interface</title>
    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>
<body>
    <!-- Your chatbot HTML goes here -->
    <!-- Bootstrap JS, Popper.js, and jQuery -->
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.7.12/umd.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>

<div class="container mt-4">
    <div class="row">
        <div class="col-md-8 offset-md-2">
            <div class="card">
                <div class="card-header bg-primary text-white">Ask AOU BF</div>
                <div class="card-header bg-primary text-white d-flex align-items-center justify-content-between">
                    <!-- Close Button -->
                    <button id="close-btn" class="btn btn-primary btn-sm">
                        <i class="fas fa-times"></i>
                    </button>
                    <!-- Language Toggle Button -->
                    <button id="toggle-lang-btn" class="btn btn-primary btn-sm">
                        <i class="fas fa-globe"></i>
                    </button>
                </div>
                <div class="card-body" id="chat-box" style="height: 300px; overflow-y: auto;">
                    <!-- Messages will be shown here -->
                    <div id="welcome-message">
                        Hi, I'm AOU best friend here to help you. I will do my best for you.
                    </div>
                </div>
                <div class="card-footer">
                    <div class="input-group">
                        <input type="text" id="user-input" class="form-control" placeholder="Ask a question">
                        <div class="input-group-append">
                            <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">
                            <button id="send-btn" class="btn btn-outline-secondary">
                                <i class="fa fa-arrow-right"></i>
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css">  
