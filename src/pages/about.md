---
layout: ../layouts/AboutLayout.astro

title: "Submit"
---

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Email Subscription Form</title>
<style>
#success-message {
    display: none;
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    padding: 20px;
   background-color: lightgreen;
   border: 2px solid RED;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
#success-message p {
  color: RED; /* 文本颜色为蓝色 */
  font-family: Arial, sans-serif; /* 字体为 Arial 或者 sans-serif（无衬线字体） */
}

</style>
</head>
<body>
On the seventh day of the Lunar New Year this year, while we were still immersed in the joy and busyness of the Spring Festival, OpenAI quietly made a big move, releasing Sora, a super bombshell.

On February 16th, OpenAI officially announced its first text-to-video model—Sora. The functionality and attributes of Sora are enough to astonish the world: it can directly output videos up to 60 seconds in length through text commands. These videos are not simple videos; they contain highly detailed backgrounds, complex multi-angle shots, and emotionally rich characters. This means that, following text and images, OpenAI is the first to extend advanced AI technology into the field of video.

<h2>Be the first to know when Sora is live!</h2>
<form id="subscribe-form">
  <input type="email" id="email" placeholder="Enter your email" required>
  <button type="submit">Subscribe</button>
</form>

<div id="success-message">
  <p> SUCESS THANKS FOR JOINING US!</p>
</div>

<script>
document.getElementById('subscribe-form').addEventListener('submit', function(event) {
  event.preventDefault();
  var emailInput = document.getElementById('email');
  var email = emailInput.value;
  // Here you can perform validation of the email address if needed

  // Simulating a successful subscription
  showSuccessMessage();
});

function showSuccessMessage() {
  var successMessage = document.getElementById('success-message');
  successMessage.style.display = 'block';
  setTimeout(function() {
    successMessage.style.display = 'none';
  }, 3000); // Hide the message after 3 seconds
}
</script>

</body>
</html>
