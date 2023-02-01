<script lang="ts">
    let color = 'red';
    let showText = true
    const toggle = () => {
        color = color === 'red' ? 'blue' : 'red';
        showText = !showText
    };
</script>

{#if showText}
<h1 style="color: {color}">Selected color is {color}</h1>
{:else}
<p>Show text variable is {showText}</p>
{/if}
<button on:click={toggle}>toggle color</button>