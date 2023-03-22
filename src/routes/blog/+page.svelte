<script lang="ts">
  import { base } from "$app/paths";
  import Navbar from "$lib/Navbar.svelte";
</script>

<Navbar currLoc={"/blog"} />

<div class="text-2xl font-light w-full bg-gray-400 p-16 text-center text-white">
  <h1>The</h1>
  <h1 class="font-bold uppercase">Good Answer</h1>
  <h1>Blog</h1>
</div>

<div class="w-full bg-white p-8">
  <div class="flex justify-center items-start px-8 lg:w-2/3 gap-8">
    <div class="flex-1">
      <img src={base + "/blog1.jpg"} alt="" />
      <img src="" alt="" />
    </div>
    <div class="flex-1 flex flex-col gap-4">
      <p>
        It's pretty common to hear the phrase "good question." It happens in
        conversations all the time. As a reporter, I never liked hearing that.
        Because I consider ALL my interview questions to be good questions.
      </p>
      <p>
        You don't hear the phrase Good Answer as much. Unless you're watching
        Family Feud.
      </p>
      <p>I like to explore the skills involved in crafting a "Good Answer."</p>
      <p>
        Obviously, a Good Answer must answer the question posed. And there's
        more than one good answer. But let's go deeper. In a job interview
        setting for example, A good answer isn't extemporaneous. You don't just
        "wing it" and hope it sounds like a good answer. It takes preparation.
      </p>
      <p>
        In fact, it takes some reverse engineering to fashion a Good Answer to a
        Good Question. A Good Answer is your unique blend of honesty, humility
        and understanding in anticipation of a question. And it better not sound
        memorized.
      </p>
      <p>
        In my career, I've interviewed thousands of people. I've heard good
        answers and crummy ones. Here's some advice on composing a compelling
        and credible <b>Good Answer</b>.
      </p>
    </div>
  </div>
</div>
<div class="w-full bg-kbcgold p-8 grid grid-cols-1 place-items-center">
  <div class="w-2/3">
    <h2 class="text-center font-bold text-2xl">Do your Homework</h2>
    <p class="py-4">
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
    <div class="w-full grid grid-cols-1 place-items-center py-8">
      <button class=" bg-kbcblue text-white font-bold text-center px-16 py-2"
        >Read Full Article</button
      >
    </div>
  </div>
</div>
