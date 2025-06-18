body {
  background-color: #f7f3e9;
  font-family: 'Georgia', serif;
  color: #4e4e4e;
  text-align: center;
  padding: 50px;
}
button {
  background-color: #c7d8b6;
  color: #333;
  border: none;
  padding: 15px;
  margin: 10px;
  border-radius: 10px;
  cursor: pointer;
}
button:hover {
  background-color: #b0c8a4;
}
<!DOCTYPE html>
<html>
<head>
  <title>How Do You Feel Today?</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <h1>How Do You Feel Today?</h1>
    <button onclick="showResponse('happy')">😊 Happy</button>
    <button onclick="showResponse('sad')">😢 Sad</button>
    <button onclick="showResponse('anxious')">😟 Anxious</button>
    <p id="response"></p>
  </div>
  <script src="script.js"></script>
</body>
</html>
function showResponse(feeling) {
  const messages = {
    happy: "🌼 That's beautiful. What’s something that made you smile today?",
    sad: "💧 It’s okay to feel this way. Write down what’s weighing on your heart.",
    anxious: "🌿 Breathe. You're safe. What thoughts are racing through your mind?",
  };
  document.getElementById('response').innerText = messages[feeling];
}
