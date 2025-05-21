<script lang="ts">
    const cartoonImg = '/images/giblie-me.png'
</script>

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
        color: #FFF;
        margin: 0;
    }

    #bio-section p {
        font-family: "Inconsolata", monospace;
        font-size: 2rem;
        color: #f8bfe7;
        font-weight: 600;
        margin: 0;
    }

    #main-section-right {
        
        background-image: url('images/giblie-me.png');
        background-size: cover;
    }

    .main-section-segment {
        width: 50%;
        height: 100%;
    }
</style>



<section id="main">
    <div id="main-section-left" class="main-section-segment">
        <div id="bio-section">
            <h2>Full Stack</h2>
            <h2>Developer.</h2>
            <p>If it is creative, I am interested.</p>
        </div>
    </div>
    <div id="main-section-right" class="main-section-segment"></div>
</section>


