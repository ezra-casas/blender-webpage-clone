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
    let current = true;
</script>

<nav>
    <div>
        <h1>Blender Logo</h1>
    </div>
    <div class="nav-items">
       {#each navigations as page}
            <a
                class="{current === true ? 'selected' : ''}"
                href="/{page.value}">{page.name}</a>
        {/each}
    </div>

</nav>

<style>
    nav{
        display: flex;
        justify-content: space-around;
        align-items: center;
    }
    .nav-items{
        display: flex;
        justify-content: space-between;
    }
    h1{
        color: lightcoral;
    }
</style>

<slot></slot>