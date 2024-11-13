<div>
  <pre><code id="codeText">https://github.com/sanjeev249-cry/portfolio</code></pre>
  <button onclick="copyText()">Copy to Clipboard</button>
</div>

<script>
function copyText() {
  // Get the text from the <code> element
  const codeText = document.getElementById("codeText").textContent;

  // Use the Clipboard API to copy the text
  navigator.clipboard.writeText(codeText).then(() => {
    alert("Copied to clipboard!");
  }).catch(err => {
    console.error("Could not copy text: ", err);
  });
}
</script>
