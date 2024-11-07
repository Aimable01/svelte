<script>
  import { onDestroy, onMount } from "svelte";

    onMount(() => console.log("Mounted home page"))
    onDestroy(() => console.log("unmounted home page"))
</script>


<nav>
   <ul>
     <li>
        <a href="/">Home</a>
    </li>
    <li>
        <a href="/posts">Posts</a>
    </li>
   </ul>
</nav>

<h1>Home page</h1>