<script lang="ts">
    const products = [
        { id: "a1a2", name: 'Svelte' },
        { id: "b1b2", name: 'React' },
        { id: "c1c2", name: 'Vue' },
    ];
</script>

{#each products as product, i}
    <div>index: {i}, ID: {product.id}, name: {product.name}</div>
{/each}
