<script lang="ts">
  const logo = "logo.png";

  import { Github, Linkedin } from "@lucide/svelte";
</script>

<header>
  <img id="header-logo" src={logo} alt="" />
  <nav id="navigation-section">
    <ul>
      <li>Blog</li>
      <li>Projects</li>
      <li>Contact</li>
    </ul>
  </nav>
</header>
<section id="main">
  <div id="main-section-left" class="main-section-segment">
    <div id="bio-section">
      <h2>Full Stack</h2>
      <h2>Developer.</h2>
      <p>If it is creative, I am interested.</p>

      <span class="icon">
        <Github size={40} />
      </span>

      <span class="icon">
        <Linkedin size={40} />
      </span>
    </div>
  </div>
  <div id="main-section-right" class="main-section-segment"></div>
</section>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background-color: #a57992;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
  }

  :global(img) {
    max-width: 100%;
  }

  :global(li) {
    list-style: none;
  }

  .icon {
    margin-right: 5px;
  }

  .icon:hover {
    cursor: pointer;
    color: #fff;
  }

  header {
    width: 80%;
    display: flex;

    align-items: center;
  }

  header img {
    width: 150px;
  }

  #navigation-section ul {
    display: flex;
    font-family: "Inconsolata";
  }

  #navigation-section li {
    font-size: 2rem;
    margin-right: 1em;
    color: #fff;
  }

  #navigation-section li:hover {
    text-decoration: underline;
  }

  #main {
    width: 80%;
    height: 800px;
    display: flex;
  }

  #main-section-left {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  #bio-section {
    width: 50%;
  }

  #bio-section h2 {
    font-family: "Poetsen One", sans-serif;
    font-size: 3.1rem;
    color: #fff;
    margin: 0;
  }

  #bio-section p {
    font-family: "Inconsolata", monospace;
    font-size: 2rem;
    color: #f8bfe7;
    font-weight: 600;
    margin: 0 0 15px 0;
  }

  #main-section-right {
    background-image: url("images/giblie-me.png");
    background-size: cover;
  }

  .main-section-segment {
    width: 50%;
    height: 100%;
  }
</style>
