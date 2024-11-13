html
<div>
  <pre>
    <code id="codeBlock">[link]https://github.com/sanjeev249-cry/portfolio</code>
  </pre>
  <button onclick="copyToClipboard()">Copy to Clipboard</button>
</div>

<script>
function copyToClipboard() {
  const codeBlock = document.getElementById("codeBlock").textContent;
  navigator.clipboard.writeText(codeBlock).then(() => {
    alert("Copied to clipboard!");
  });
}
</script>

this repo contanins complete html and css resume template
