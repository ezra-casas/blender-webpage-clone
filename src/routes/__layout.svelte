<script>
    const navigations = [
        {name: "home", value: "home", active: true},
        {name: "Features", value: "features", active: false},
        {name: "Download", value: "download", active: false},
        {name: "Support", value: "support", active: false},
        {name: "Get Involved", value: "get_involved", active: false},
        {name: "About", value: "about", active: false},
        {name: "Jobs", value: "jobs", active: false},
        {name: "Store", value: "store", active: false},
    ]
</script>

<nav>
    <div>

    </div>
    {#each navigations as page}
        <a href="/{page.value}">{page.name}</a>
    {/each}
</nav>

<style>
    nav{
        display: flex;
        justify-content: space-around;
    }
</style>
<slot></slot>