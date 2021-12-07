<script>
    import data from '$lib/data/stories.json';
    console.log(data);
    import '@fontsource/barlow';
   

</script>

<h1><strong>Customer Stories</strong></h1>

<section class="filters-grid">
    <div class="tag-holder-bar">
        <p class="tag">Next.js</p>
        <p class="tag">Dynamic Sites</p>
        <p class="tag">Vercel ⚔️</p>
        <p class="tag">WP Migration</p>
        <p class="tag">Self-serve Upsell</p>
        <p class="tag">Azure</p>
        <p class="tag">Monolith</p>
        <p class="tag">Shopify</p>
    </div>
</section>

<section class="stories">
    {#each data as { company, tags, industry, project, whyImportant, whyStatusQuoBad, quantifiedResults}, index}
        <a href="/peloton">
            <div class="story-snippet">
                <h2>{company}</h2>
                <div class="tag-holder">
                    {#each tags as tag}
                        <p class="tag">{tag}</p>
                    {/each}
                </div>
                <p class="industry"><em>{industry}</em></p>
                <p>{project}..</p>
            </div>
        </a>

    {/each}
</section>



<style>
    h1 {
        font-size: 2.5rem;
    }
    .stories {
        font-family: 'Barlow';
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        column-gap: 1rem;
        row-gap: 2rem;
        padding: 1.5rem 3rem 3rem;
    }

    .stories a {
        text-decoration: none;
    }

    .story-snippet {
        background-color:  rgba(11, 0, 14, 0.61);
        padding: 9px;
        border-radius: 5px;
    }

    .story-snippet h2 {
        font-size: 2rem;
        
    }

    .tag-holder {
        display: flex;
        flex-direction: row;

    }
    .tag-holder-bar {
        display: flex;
        flex-direction: row;
        justify-content: center;
    }

    .tag {
        margin: 2.5px;
        padding: 3px;
        border-radius: 5px;
        background-color: grey;
        text-decoration: none;
    }

    .industry {
        color: grey;
    }

</style>