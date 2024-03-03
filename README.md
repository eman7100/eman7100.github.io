<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chatbot Interface</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="chat-container">
    <div id="chat-messages" class="chat-messages">
        <!-- Chat messages will be displayed here -->
    </div>
    <form id="chat-form" class="chat-form">
        <input type="text" id="chat-input" class="chat-input" placeholder="Type your message here..." required>
        <button type="submit" class="send-button">Send</button>
    </form>
</div>

<script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
}
.chat-container {
    width: 300px;
    height: 500px;
    border: 1px solid #ccc;
    display: flex;
    flex-direction: column;
}
.chat-messages {
    flex: 1;
    padding: 10px;
    overflow-y: auto;
    border-bottom: 1px solid #ccc;
}
.chat-form {
    display: flex;
}
.chat-input {
    flex: 1;
    padding: 10px;
    border: none;
    border-right: 1px solid #ccc;
}
.send-button {
    padding: 10px;
    border: none;
    background-color: #007bff;
    color: white;
    cursor: pointer;
}
.send-button:hover {
    background-color: #0056b3;
}
document.getElementById('chat-form').addEventListener('submit', function(e) {
    e.preventDefault(); // Prevent form from submitting normally
    var inputField = document.getElementById('chat-input');
    var message = inputField.value;
    displayMessage(message);
    inputField.value = ''; // Clear input field after sending
});

function displayMessage(message) {
    var chatMessages = document.getElementById('chat-messages');
    var messageElement = document.createElement('div');
    messageElement.textContent = "You: " + message;
    chatMessages.appendChild(messageElement);
    
    // Simulate a chatbot response
    var responseElement = document.createElement('div');
    responseElement.textContent = "Chatbot: Echoing - " + message;
    setTimeout(() => chatMessages.appendChild(responseElement), 500); // Delay the bot response for realism
}
