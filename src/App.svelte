<script lang="ts">
    export let name: "Adam" | "Eve" | "Snake" | "God" | "Goat Person";
</script>

<main>
    <h1>Hello {name}!</h1>
    <button
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
