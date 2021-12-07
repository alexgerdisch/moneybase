<script>
    import '@fontsource/barlow';
</script>

<section class="fullstory">
    <div class="title-bar">
        <img class="logo" src="Peloton_logo_PNG7.png" alt="Peloton" />
    </div>
    <div class="tag-holder">
        <p class="tag">Next.js</p>
        <p class="tag">Dynamic Sites</p>
        <p class="tag">Vercel ⚔️</p>
    </div>
    
    <p>-------------------------------------------------</p>
    
    <p class="story-text">Raj Nigam, Frontend Developer, wanted to quickly build a new site for Peloton without using infra resources.</p>
    <p class="story-text">This was important becuase as a hyper growth startup, they needed to have a quick dev workflow, the ability to build and host reliably without any downtime, and an easy to manage stack.</p>
    <p class="story-text">They could not accomplish this using Cloudflare, etc because their infra stack required constant mantenence and a dedicated team. It limited the ability of their cross functional teams (marketing, content, eng, support) to get things done.</p>
    <p class="story-text">Now, Peloton has standardized on a jamstack architecture using Netlify. Their team of 200+ devs deploys 1300 times a day across 75 unique sites.</p>
    
</section>




<style>

    .fullstory {
        width: 760px;
        flex-direction: column;
        
    }

    .title-bar {
        display: flex;
        flex-direction: row;
    }

    .logo {
        display: flex;
        width: 400px;
        
    }
    .tag-holder {
        display: flex;
        flex-direction: row;

    }

    .tag {
        margin: 2.5px;
        padding: 3px;
        border-radius: 5px;
        background-color: grey;
        text-decoration: none;
    }

    .story-text {
        font-size: 1.5rem;
    }
</style>