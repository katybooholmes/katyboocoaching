<script lang="ts">
  const navItems = [
    { label: "Home", href: "/" },
    { label: "About", href: "/about" },
    { label: "How it Works", href: "/how" },
    { label: "Resume Writing", href: "/resume" },
    { label: "Contact", href: "/contact" },
    { label: "Testimonials", href: "/testimonials" },
    { label: "Blog", href: "/blog" },
  ];

  const goHome = () => {
    window.location.assign("/");
  };

  export let currLoc: string;
  console.log(currLoc);
</script>

<div
  class="static flex w-full md:sticky top-0 overflow-x-clip px-4 flex-col md:flex-row bg-white justify-center align-center md:justify-start z-10 border-blue-800 border-b-2"
>
  <nav class=" m-auto">
    <div class="flex w-full px-5 m-auto box-border items-center h-full">
      <ul class="flex flex-col md:flex-row">
        <button on:click={goHome}>
          <!--insert svg logo here-->
        </button>
        <li class="px-4" />
        {#each navItems as item}
          <li class="bg-white text-kbcblue my-2 md:m-2 md:p-2 md:my-6">
            {#if item.href === currLoc}<a
                class="box-border border-kbcblue rounded-lg hover:border-t-2 p-2 hover:border-b-2 font-bold"
                href={item.href}>{item.label}</a
              >
            {:else}
              <a
                class="box-border border-kbcblue rounded-lg hover:border-t-2 p-2 hover:border-b-2 "
                href={item.href}>{item.label}</a
              >
            {/if}
            <hr class="visible md:hidden mt-4" />
          </li>
        {/each}
      </ul>
    </div>
  </nav>
</div>
