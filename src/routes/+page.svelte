<script>
  import { Button } from "$lib/components/ui/button/index.js";

  const posts = [
    {
      title: "blog post title here",
      date: "6/9/1969",
      link: "/blog/test",
    },
    {
      title: "blog post title here",
      date: "6/7/1967",
      link: "/blog/1967",
    },
  ];
</script>

<div class="container mx-auto p-4 mt-15 max-w-3xl">
  <h2 class="text-4xl border w-[40px] h-[40px] flex align-items justify-center font-['Leckerli One', serif]">d</h2>
  <div class="mb-6 flex items-center justify-between">
    <h1 class="text-2xl font-bold">dromothepig</h1>
  </div>
  <p class="mb-6">Greetings, welcome to my website.</p>
  <p class="mb-6">
    I am a <a href="https://nextjs.org" target="_blank">nextjs</a> and
    <a href="https://svelte.dev/" target="_blank">sveltekit</a> fullstack software
    developer. I enjoy developing and designing web applications.
  </p>
  <p class="mb-6">
    This is my fourth year doing web development. Throughout the years, I have
    learned <a href="https://www.python.org/" target="_blank">Python</a>,
    <a href="https://nodejs.org/en" target="_blank">Javascript</a>,
    <a href="https://www.typescriptlang.org/" target="_blank">Typescript</a>,
    and <a href="https://www.rust-lang.org/" target="_blank">Java</a>. I
    primarily do web development and designing web applications with
    <a href="https://tailwindcss.com" target="_blank">Tailwind CSS</a> or pure CSS.
  </p>
  <p class="mb-6">
    Also, I have experience with databases such as
    <a href="https://www.mongodb.com/" target="_blank">MongoDB</a>,
    <a href="https://www.postgresql.org/" target="_blank">PostgreSQL</a>, and
    <a href="https://redis.io/" target="_blank">Redis</a>
  </p>
  <p class="mb-6">
    On the side, I enjoy 3D modeling with <a
      href="https://www.blender.org/"
      target="_blank">Blender</a
    >
    and making games in <a href="https://unity.com/" target="_blank">Unity</a>.
    You can find me on Discord and Github!
  </p>
  <h2 class="text-xl font-bold mb-6">Recent Posts</h2>
  {#each posts as post}
    <a href={post.link} class="no-underline hover:text-black">
      <div class="blog-post">
        <div>{post.date}</div>
        <div class="text-right">{post.title}</div>
      </div>
    </a>
  {/each}
</div>
