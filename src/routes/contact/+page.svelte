<script lang="ts"></script>

<main id="main">
  <div id="main-section-left" class="main-section-segment">
    <form action="" id="enquiry-form">
      <label for="name">Name: </label>
      <input type="text" name="name" id="name" />

      <label for="email">Email: </label>
      <input type="text" name="email" id="email" />

      <label for="enquiry">Message: </label>
      <textarea name="enquiry" id="enquiry"></textarea>

      <input type="submit" value="Get In Touch!" />
    </form>
  </div>
  <div id="main-section-right" class="main-section-segment"></div>
</main>

<style>
  #main {
    width: 80%;
    height: 800px;
    display: flex;
    border: 1px solid white;
  }

  .main-section-segment {
    width: 50%;
    height: 100%;
  }

  #main-section-right {
    background-image: url("images/giblie-me.png");
    background-size: cover;
  }

  #main-section-left {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  #enquiry-form {
    width: 80%;
    height: 60%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: #27262c;
    border-radius: 15px;
  }
</style>
