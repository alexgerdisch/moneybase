<script>
    import data from '$lib/data/stories.json';
    console.log(data);
    import '@fontsource/barlow';
   
</script>

<h1>Customer Stories</h1>

<section class="stories">
    {#each data as { company, tags, industry, project, whyImportant, whyStatusQuoBad, quantifiedResults}, index}
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

    {/each}
</section>

<section class="modal-overlay">

</section>


<style>
    .stories {
        font-family: 'Barlow';
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        column-gap: 1rem;
        row-gap: 2rem;
        padding: 1.5rem 3rem 3rem;
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

    .tag {
        margin: 2px;
        padding: 3px;
        border-radius: 5px;
        background-color: grey;
    }

    .industry {
        color: grey;
    }

</style>