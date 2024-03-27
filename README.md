# Main
All My Main Scripts

<!-- HTML code snippet in README.md -->
<pre>
  <code id="codeSnippet">
    function helloWorld() {
      console.log("Hello, world!");
    }
    helloWorld();
  </code>
</pre>
<button onclick="copyCode()">Copy code</button>

<!-- JavaScript to copy the code -->
<script>
  function copyCode() {
    var codeElement = document.getElementById('codeSnippet');
    var range = document.createRange();
    range.selectNode(codeElement);
    window.getSelection().removeAllRanges();
    window.getSelection().addRange(range);
    document.execCommand('copy');
    window.getSelection().removeAllRanges();
    alert('Code copied to clipboard!');
  }
</script>
