<script>
  import { onDestroy, onMount } from "svelte";

    onMount(() => console.log("Mounted posts page"))
    onDestroy(() => console.log("unmounted posts page"))
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

<h1>Posts page</h1>