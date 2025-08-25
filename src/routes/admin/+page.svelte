<script lang="ts">
  import { Input } from "$lib/components/ui/input/index.js";
  import { Button } from "$lib/components/ui/button/index.js";
</script>

<main class="mt-64 w-94 text-4xl">
  <h1 class="header text-4xl">admin panel</h1>
  <form>
    <Input type="email" placeholder="email" class="mb-2 w-full" required />
    <Input type="password" placeholder="password" class="mb-2 w-full" required />
    <Button type="button" class="w-full" disabled={false}>login</Button>
  </form>
</main>
