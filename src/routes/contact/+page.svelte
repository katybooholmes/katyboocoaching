<script lang="ts">
  import Navbar from "$lib/Navbar.svelte";

  let confirmCopy: string = "Click to copy";
  const copyEmail = () => {
    navigator.clipboard.writeText("katy@katyboocoaching.com");
    confirmCopy = "Copied!";
    sleep(2000).then(() => {
      confirmCopy = "Click to copy";
    });
  };

  function sleep(ms: number) {
    return new Promise((resolve) => setTimeout(resolve, ms));
  }
</script>

<Navbar currLoc={"/contact"} />

<div
  class="w-full flex justify-center bg-[url('/contactheader.jpg')] bg-cover bg-no-repeat bg-top text-center text-4xl font-bold p-32"
>
  <div class="">Let's Meet</div>
</div>

<div class="bg-white w-full flex justify-center">
  <div class="w-2/3 text-center">
    <p class="py-8">
      I look forward to working with you at this very exciting time of your
      life! You are ready to set sail into the career you have been working so
      hard for. Let's prepare you to land that DREAM job.
    </p>
    <p>You can contact me and I will get back to you right away!</p>
    <h2 class="font-bold text-2xl pt-4">Katy Boo</h2>
    <h2 class="font-bold text-2xl">cell: 612-719-7782</h2>
    <h2 class="font-bold text-2xl pb-4">
      email: <button
        class="font-bold text-2xl hover:underline "
        on:click={copyEmail}>{confirmCopy}</button
      >
    </h2>
    <p>In-person appointments: 5816 Long Brake Trail, Minneapolis, MN 55439</p>
    <p class="pt-2">
      twitter: <a
        class="hover:underline text-kbcblue"
        href="https://twitter.com/katyboocoaching">@katyboocoaching</a
      >
    </p>
    <p>
      facebook: <a
        class="hover:underline text-kbcblue"
        href="https://facebook.com/katyboocoaching">/katyboocoaching</a
      >
    </p>
  </div>
</div>
