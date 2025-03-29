<script>
    import { page } from "$app/stores";
    import "$lib/style.css";
</script>

<svelte:head>
    <link rel="icon" type="image/x-icon" href="/favicon.ico" />
</svelte:head>

<slot />
{#if $page.url.pathname == "/" || $page.url.pathname == "/admin"}
    <p
        style="color: var(--text-color-darkest); font-size: 13px; display: flex; align-items: center; justify-content: center;"
    >
        Confused? Lost? Perhaps&nbsp;<a
            href={$page.url.pathname == "/" ? "/admin" : "/"}
            style="text-decoration: underline; color: var(--text-color-darkest);"
            >{$page.url.pathname == "/"
                ? "you are an admin"
                : "you are a mere mortal"}</a
        >
    </p>
{/if}
