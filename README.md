- 👋 Hi, I’m @Malik-Shery
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Malik-Shery/Malik-Shery is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>YouTube Multi-Tab Launcher</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin: 20px;
    }
    input, button {
      padding: 10px;
      font-size: 16px;
      margin: 10px;
    }
  </style>
</head>
<body>
  <h1>YouTube Multi-Tab Launcher</h1>
  <p>Enter a YouTube video link below and open it in 10 tabs:</p>
  <input type="url" id="youtube-link" placeholder="Enter YouTube URL" required>
  <br>
  <button onclick="openTabs()">Open in 10 Tabs</button>

  <script>
    function openTabs() {
      const videoUrl = document.getElementById('youtube-link').value.trim();

      // Validate YouTube URL
      if (!videoUrl || !videoUrl.includes("youtube.com/watch")) {
        alert("Please enter a valid YouTube video URL.");
        return;
      }

      // Open video in 10 tabs
      for (let i = 0; i < 10; i++) {
        window.open(videoUrl, '_blank');
      }
    }
  </script>
</body>
</html>
