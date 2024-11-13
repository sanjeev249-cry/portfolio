<a href="#" onclick="copyLink(event)">https://github.com/username/repo.git</a>

<script>
function copyLink(event) {
  event.preventDefault(); // Prevents the link from actually navigating
  
  // Define the text you want to copy
  const linkText = "https://github.com/username/repo";

  // Copy text to clipboard
  navigator.clipboard.writeText(linkText).then(() => {
    alert("Link copied to clipboard!");
  }).catch(err => {
    console.error("Failed to copy: ", err);
  });
}
</script>



