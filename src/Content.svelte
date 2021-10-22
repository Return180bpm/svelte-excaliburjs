<!--
	@component
	### App component

	@param name: string 
	
-->
<script lang="ts" context="module">
    // export type Name = "Adam" | "Eve" | "Snake" | "God" | "Goat Person";
    // export type Name = ["Adam" , "Eve" , "Snake" , "God" , "Goat Person"];
</script>

<script lang="ts">
    // export let name: Name;
    export let foo: number;
    export let namePool = [
        "Adam",
        "Eve",
        "Snake",
        "God",
        "Goat Person",
    ] as const;
</script>

<main>
    <h1>Hello {namePool[foo]}!</h1>
    <button
        on:click={() => (foo = Math.floor(Math.random() * namePool.length))}
        class="text-red-400 uppercase bg-transparent p-3 border-2 border-red-400 rounded-2xl hover:text-red-700 hover:border-red-700"
        >Regenerate</button
    >
</main>

<style global lang="postcss">
    @tailwind base;
    @tailwind components;
    @tailwind utilities;

    main {
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
    }

    h1 {
        color: #ff3e00;
        text-transform: uppercase;
        font-size: 4em;
        font-weight: 100;
    }

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>
