<script lang="ts">
  import Navbar from "$lib/Navbar.svelte";
  const images = [
    "/logos.jpg",
    "/Unknown.png",
    "/Unknown-1.jpeg",
    "/Unknown-2.jpeg",
    "/Unknown-2.png",
    "/Unknown-3.png",
    "/Unknown-4.jpeg",
    "/Unknown-4.png",
    "/Unknown-5.png",
    "/Unknown-6.png",
    "/Unknown-7.png",
  ];
</script>

<Navbar currLoc={"/about"} />

<div class="grid grid-cols-2 place-items-center h-64">
  <div
    class="absolute w-full px-8 md:px-32 py-32 bg-[url('/mnskyline.jpg')] brightness-50 bg-no-repeat bg-cover bg-top"
  />
  <h1 class="text-4xl font-bold text-white brightness-200 z-10">
    What's <i>your</i> story?
  </h1>
  <img
    src="/headshot.jpg"
    alt="headshot"
    class="rounded-full w-48 z-10 border-white border-2"
  />
</div>
<div
  class="w-full bg-white px-8 md:px-32 py-8 flex flex-col gap-4 xl:text-center"
>
  <p>
    I've spent 30+ years on both sides of the camera. As a TV reporter, I
    interviewed execs and professionals, athletes and rock stars, politicians
    and plain old people.
  </p>
  <p>
    I've dedicated my career to helping people communicate their unique stories.
    I believe the stories that make the greatest impact are honest and credible,
    engaging and entertaining.
  </p>
  <p>
    <b>Fun fact:</b> Dolly Parton and I enjoyed sweet tea together after our interview
    in Dollywood, TN.
  </p>
</div>
<div class="w-full grid grid-cols-1 place-items-center">
  <div
    class="w-full bg-white flex flex-row justify-center gap-8 px-8 md:px-32 py-8 xl:w-1/2"
  >
    <div class="flex-1 grid grid-cols-3 items-center justify-items-center">
      {#each images as image}<img src={"/logos" + image} alt="logos" />{/each}
    </div>
    <div class="flex-1 flex flex-col gap-4">
      <h1 class="font-bold text-2xl">Master Interviewer</h1>
      <p>
        I've interviewed scientists, exploreres and environmentalists for <b
          >National Geographic</b
        >. I interviewed influencers for <b>Oprah</b>'s 2020 National Tour.
      </p>
      <p>
        For home makeover shows on <b>HGTV</b> and <b>DIY</b>, I've interviewed
        tv stars and regular folks looking for 15 minutes of fame and a new
        bathroom. I interviewed interesting people in exotic locations for
        <b>The Travel Channel</b>. My work for <b>Animal Planet</b> included interviewing
        dog owner and their dogs. The dogs were way cooler.
      </p>
      <p>
        When I was interviewing on the campaign trail, Jesse Ventura taught me a
        sweet thumb wrestling move. He was a pro wrestler. And then Minnesota's
        governor.
      </p>
    </div>
  </div>
</div>
<div
  class="w-full bg-[url('/aboutbgstock.jpg')] bg-no-repeat bg-cover bg-bottom px-8 md:px-32 py-16"
>
  <div class="w-2/3 bg-white p-8 flex flex-col gap-4">
    <h1 class="text-2xl font-bold">Experienced Media Trainer</h1>
    <p>
      I've media coached high-profile lawyers and Mayo Clinic doctors. I'll
      admit, all the doctors I coached were super intelligent, but they
      definitely needed guidance on refining their messages and keeping it
      brief.
    </p>
    <p>
      I have a master's degree in broadcast journalism from Northwestern
      University's Medill School of Journalism. My master's program included
      working in Washington, DC where I covered stories at the White House and
      the Capitol.
    </p>
    <p>I have a BA in Speech/Communications from Boston College.</p>
    <p>
      I live in the Twin Cities. You might find me walking around one of the
      lakes. Or working on my latest project: hand-painting cool signs on
      century-old reclaimed barnwood. <a
        class="text-kbcblue hover:underline"
        href="https://www.reclaimedwords.com">www.reclaimedwords.com</a
      >
    </p>
  </div>
</div>
<div class="w-full bg-kbcgold flex py-8 justify-center">
  <div class="md:w-1/2">
    <h1 class="text-xl font-bold pb-4">What does this all mean for you?</h1>
    <p>
      My vast experience can help you identify and illuminate <i>your</i> story so
      you can be prepared to shine in your next interview.
    </p>
  </div>
</div>
