<script lang="ts">
  import { Github, Linkedin } from "@lucide/svelte";
  import giblieMe from "../../../static/images/giblie-me.png";
</script>

<main id="main">
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
  <div id="main-section-right" class="main-section-segment">
    <div id="photo-container"></div>
  </div>
</main>

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
    max-width: 1900px;
    margin: 0 auto;
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
  }

  #main {
    width: 80%;
    height: 800px;
    display: flex;
  }

  .main-section-segment {
    width: 50%;
    height: 100%;
  }

  #main-section-left {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  #main-section-right {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  #photo-container {
    height: 400px;
    width: 400px;
    background-image: url("/static/images/giblie-me.png");
    background-size: cover;
  }
  #bio-section {
    width: 50%;
    animation-duration: 1s;
    animation-name: slide-in;
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

  @keyframes slide-in {
    from {
      translate: -20vw 0;
      scale: 150% 1;
      opacity: 0;
    }

    to {
      translate: 0 0;
      scale: 100% 1;
      opacity: 1;
    }
  }
</style>
