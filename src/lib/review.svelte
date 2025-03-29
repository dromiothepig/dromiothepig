<script>
    export let author = "Anonymous";
</script>

<div style="background-color: var(--background-lighter); border: 1px solid var(--background-lightest); padding: 1em; margin: 1em; border-radius: 5px;">
    {author}: <slot />
</div>