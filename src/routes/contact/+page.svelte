<script lang="ts"></script>

<main id="main">
  <div id="main-section-left" class="main-section-segment">
    <form action="" id="enquiry-form" autocomplete="off">
      <h2 id="form-heading">Hey There!</h2>
      <label for="name">Name: </label>
      <input type="text" name="name" id="name" />

      <label for="email">Email: </label>
      <input type="text" name="email" id="email" />

      <label for="enquiry">Message: </label>
      <textarea name="enquiry" id="enquiry"></textarea>

      <input type="submit" value="Get In Touch!" id="submit-btn" />
    </form>
  </div>
  <div id="main-section-right" class="main-section-segment">
    <div id="photo-container"></div>
  </div>
</main>

<style>
  #main {
    width: 80%;
    height: 800px;
    display: flex;
  }

  .main-section-segment {
    width: 50%;
    height: 100%;
  }

  #main-section-right {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  #main-section-left {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  #photo-container {
    height: 400px;
    width: 400px;
    background-image: url("/static/images/giblie-me.png");
    background-size: cover;
  }

  #form-heading {
    color: pink;
    font-family: "Poetsen One", sans-serif;
    font-size: 4rem;
  }

  #enquiry-form {
    width: 60%;
    height: 85%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: #27262c;
    border-radius: 15px;
    font-family: Inconsolata;
  }
  label,
  input,
  textarea {
    color: pink;
    font-size: 1.2rem;
    width: 70%;
    padding: 0.2em;
  }

  input,
  textarea {
    background-color: #27262c;
    border: 4px solid pink;
  }

  label {
    font-size: 1.5rem;
    font-weight: 500;
  }

  input {
    height: 30px;
  }

  textarea {
    height: 90px;
  }

  #submit-btn {
    padding: 0.45em;
    font-size: 1.3em;
    margin-top: 1em;
    height: 50px;
    width: 73%;
  }

  #submit-btn:hover {
    cursor: pointer;
    background-color: #333236;
  }
</style>
