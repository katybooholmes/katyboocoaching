<script lang="ts">
  import { base } from "$app/paths";
  import Navbar from "$lib/Navbar.svelte";
</script>

<Navbar currLoc={"/blog"} />

<div
  class="text-2xl font-light w-full bg-[url('/blogheader.jpg')] bg-no-repeat bg-cover p-16 text-center text-white"
>
  <h1>The</h1>
  <h1 class="font-bold uppercase">Good Answer</h1>
  <h1>Blog</h1>
</div>

<div class="w-full bg-white p-8">
  <div class="grid grid-cols-1 md:flex justify-center items-start px-8 gap-8">
    <div class="flex-1 flex flex-col place-items-end">
      <img class="p-4" src={base + "/blog1.jpg"} alt="" />
    </div>
    <div class="flex-1 flex flex-col gap-4 place-items-center">
      <p class="w-full">
        It's pretty common to hear the phrase "good question." It happens in
        conversations all the time. As a reporter, I never liked hearing that.
        Because I consider ALL my interview questions to be good questions.
      </p>
      <p class="w-full">
        You don't hear the phrase Good Answer as much. Unless you're watching
        Family Feud.
      </p>
      <img class=" w-64" src="/steveharvey.jpeg" alt="" />
      <p class="w-full">
        I like to explore the skills involved in crafting a "Good Answer."
      </p>
      <p class="w-full">
        Obviously, a Good Answer must answer the question posed. And there's
        more than one good answer. But let's go deeper. In a job interview
        setting for example, A good answer isn't extemporaneous. You don't just
        "wing it" and hope it sounds like a good answer. It takes preparation.
      </p>
      <p class="w-full">
        In fact, it takes some reverse engineering to fashion a Good Answer to a
        Good Question. A Good Answer is your unique blend of honesty, humility
        and understanding in anticipation of a question. And it better not sound
        memorized.
      </p>
      <p class="w-full">
        In my career, I've interviewed thousands of people. I've heard good
        answers and crummy ones. Here's some advice on composing a compelling
        and credible <b>Good Answer</b>.
      </p>
    </div>
  </div>
</div>
<div class="w-full bg-kbcgold p-8 grid grid-cols-1 place-items-center">
  <div class="w-2/3 grid grid-cols-1 gap-4">
    <h2 class="text-center font-bold text-2xl">Do your Homework</h2>
    <p>
      Just because you graduated from college and you're in the "real world"
      doesn't mean you're finished with homework. In fact, if you want to land a
      good job, your homework is more important than ever.
    </p>
    <p>
      Statistics show the job market is fierce. For every 250 corporate jobs,
      hiring managers grant 4-6 interviews. That's all for one job. The stakes
      are high. If you are one of the lucky ones to get a job interview, you
      better make it count.
    </p>
    <p>
      As an interview coach, one of the areas I cover is Research. As in,
      researching your prospective company. If you don't do your homework before
      your interview, it shows. Hiring managers say one of their biggest pet
      peeves is when candidates ask questions that are clearly on the company
      website.
    </p>
    <p>
      Ed Huerta-Margotta, Director of Recruiting at Carmichael Lynch Creative Ad
      Agency, says if you ask him what clients he has, your interview is
      essentially dead in the water. Every company has a website. He says, "If
      you're passionate about working with us, you should pore over our website
      and work to learn as much as you can about us."
    </p>
    <p>
      The candidates that shine are the ones who can talk intelligently about
      the company. Being unprepared looks unprofessional. In a situation where
      you need every advantage, thoroughly researching the company is mandatory.
    </p>
    <p>
      Gone are the days of cramming for tests, but homework is here to stay. In
      order to be in the running for your ideal job, you better be able to prove
      to hiring managers that you've done your research.
    </p>
    <!-- <div class="w-full grid grid-cols-1 place-items-center py-8"> -->
    <!--   <a -->
    <!--     href="https://www.tumblr.com/katybooholmes" -->
    <!--     target="_blank" -->
    <!--     class=" bg-kbcblue text-white font-bold text-center px-16 py-2" -->
    <!--     >Read Full Article</a -->
    <!--   > -->
    <!-- </div> -->
  </div>
</div>
