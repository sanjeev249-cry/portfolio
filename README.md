<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Copy to Clipboard</title>
    <style>
          <div class="container">
        <p>Click the button below to copy the repository clone link:</p>
        <pre><code id="codeText">https://github.com/sanjeev249-cry/portfolio.git</code></pre>
        <button onclick="copyText()">Copy to Clipboard</button>
    </div>
     <script>
        function copyText() {
            // Get the text from the <code> element
            const codeText = document.getElementById("codeText").textContent;
      navigator.clipboard.writeText(codeText).then(() => {
                alert("Copied to clipboard!");
 }).catch(err => {
                console.error("Failed to copy: ", err);
  });
 }
 </script>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            text-align: center;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
        }
    </style>
</head>
<body>
</body>
</html>
