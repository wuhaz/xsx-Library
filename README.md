# Main
All My Main Scripts


      <section>
        <p>Copy from an element specified by the <code>for</code> attribute:</p>
        <div id="name">@hubot copied from &lt;div&gt;</div>
        <clipboard-copy for="name">
          Copy
          <span class="notice" hidden>Copied!</span>
        </clipboard-copy>
      </section>
      <hr />

      <section>
        <label>
          <p>Copy from an input element specified by the <code>for</code> attribute:</p>
          <input id="login" value="@hubot copied from &lt;input&gt;" size="40" />
        </label><br />
        <clipboard-copy for="login">
          Copy
          <span class="notice" hidden>Copied!</span>
        </clipboard-copy>
        </section>
      <hr />

      <section>
        <label>
          Paste the text here to test
          <textarea class="textarea" rows="10" cols="50"></textarea>
        </label>
      </section>
  </body>
</html>
