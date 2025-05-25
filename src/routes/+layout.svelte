<script lang="ts">
  let { children } = $props();
  const logo = "logo.png";
</script>

<header>
  <a id="icon-btn" href="/welcome"><img id="header-logo" src={logo} alt="" /></a
  >
  <nav id="navigation-section">
    <ul>
      <li><a href="/blog">Blog</a></li>
      <li><a href="/projects">Projects</a></li>
      <li><a href="/contact">Contact</a></li>
    </ul>
  </nav>
</header>

{@render children()}

<style>
  header {
    width: 80%;
    display: flex;
    align-items: center;
  }

  header img {
    width: 150px;
  }

  #navigation-section a {
    color: inherit;
    text-decoration: none;
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
</style>
