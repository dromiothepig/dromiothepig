<script>
    import { page } from "$app/stores";
</script>

<div style="text-align: center;">
    <h1>{$page.status}</h1>
    <p style="font-size: 18px;">{$page.error.message}</p>
    <a href="/" style="text-decoration: none; display: flex; justify-content: center; width: 100%;">
        <button class="accent1" style="width: 200px;">Go Back</button>
    </a>
</div>