<!DOCTYPE html>
<html>
<head>
  <title>Mood Generator</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      text-align: center;
      margin-top: 100px;
      background-color: #f0f8ff;
    }
    button {
      padding: 10px 20px;
      font-size: 18px;
      background-color: #ff69b4;
      color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }
    h1 {
      color: #333;
    }
    p {
      font-size: 24px;
      color: #444;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <h1>Mood Generator</h1>
  <button onclick="generateMood()">Click to get a random mood</button>
  <p id="moodOutput"></p>

  <script>
    const moods = ["Happy", "Sad", "Excited", "Bored", "Nervous", "Sleepy", "Confident", "Flirty"];
    
    function generateMood() {
      const mood = moods[Math.floor(Math.random() * moods.length)];
      document.getElementById("moodOutput").innerText = "You're feeling: " + mood;
    }
  </script>
</body>
</html>
