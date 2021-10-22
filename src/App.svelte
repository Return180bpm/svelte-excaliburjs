<script lang="ts">
    import Content from "./Content.svelte";
    import Workbench from "./Workbench.svelte";
</script>

<Content foo={0} />
<Workbench />

<style global lang="postcss">
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
</style>
