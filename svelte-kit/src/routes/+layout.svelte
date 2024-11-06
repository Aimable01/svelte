<script lang="ts">
    export let navLinks = [
        {link:"/", name: "Home"},
        {link:"/posts", name: "Posts"},
    ]
</script>

<nav>
   {#each navLinks as navlink}
    <a href={navlink.link}>{navlink.name}</a>
   {/each}
</nav>

<slot />