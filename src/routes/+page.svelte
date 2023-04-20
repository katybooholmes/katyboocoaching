<script lang="ts">
  import Navbar from "$lib/Navbar.svelte";
  import { base } from "$app/paths";

  const howitworksitems = [
    {
      num: "1",
      label:
        "Before we meet, send me your resume, plus job description for upcoming interview or ideal target job",
    },
    {
      num: "2",
      label:
        "I'll send you a list of commonly asked interview questions for you to review",
    },
    {
      num: "3",
      label: "We will discuss: ",
      list: [
        "meeting and greeting",
        "identifying your key messages",
        "verbal and non-verbal communication",
        "job interview followup duties",
      ],
    },
    {
      num: "4",
      label: "In-person or video mock interview with immediate feedback",
    },
  ];
</script>

<Navbar currLoc={"/"} />

<div
  class="w-full bg-[url('/homepageheader.jpg')] bg-no-repeat bg-cover bg-center p-16 py-32 md:pl-32"
>
  <h1 class="text-white text-3xl font-bold">Interview with confidence.</h1>
  <p class="text-white py-4 w-1/2">
    First job interviews can be scary. My <b>personalized preparation</b> gives
    you the <b>confidence</b> to land the right job for you.
  </p>
  <a
    href="/contact"
    class="bg-kbcgold font-bold py-2 px-16 rounded-md text-kbcblue"
    >Let's talk</a
  >
</div>
<div class="bg-kbcgold w-full py-8 grid grid-cols-1 place-items-center">
  <div class="bg-white w-2/3 md:w-1/2 p-8 text-center text-kbcblue">
    <p>
      We'll <b>strategize</b> the best way to highlight your skills and match them
      to employers' needs.
    </p>
    <p class="pt-4">
      The confidence you gain goes well beyond the next interview. <b
        >These are skills for life.</b
      >
    </p>
  </div>
</div>
<div class="bg-white w-full grid grid-cols-1 place-items-center p-8">
  <h1 class="text-center text-3xl font-bold text-kbcblue">How it Works</h1>
  <div
    class="flex flex-col md:flex-row md:justify-center p-8 md:items-start gap-8 text-kbcblue"
  >
    {#each howitworksitems as item}
      <div class="flex-1 grid grid-cols-1 place-items-center">
        <h1 class="text-7xl font-bold bg-kbcgold py-4 px-8 rounded-full">
          {item.num}
        </h1>
        <p class="pt-4 text-center">{item.label}</p>
        {#if item.list != undefined}
          <ul class="list-disc pl-8">
            {#each item.list as listitem}<li>{listitem}</li>{/each}
          </ul>
        {/if}
      </div>
    {/each}
  </div>
</div>
<div
  class="w-full bg-kbcgold p-16 md:px-32 grid grid-cols-1 md:grid-cols-2 text-kbcblue"
>
  <div class="px-8">
    <h1 class="text-3xl font-bold">Why you may need interview coaching:</h1>
    <ul class="list-disc py-8">
      <li>If you tend to get nervous, practice <i>will</i> help.</li>
      <li>
        If you get interviews but no offers, I can help you see blind spots that
        interviewers won't tell you about.
      </li>
      <li>
        <i>Non-verbal communications:</i> your facial and body language speak volumes
        even if you don't say a word.
      </li>
    </ul>
    <a href="/contact" class="bg-kbcblue px-8 py-2 text-white rounded-lg"
      >Schedule a session</a
    >
  </div>
  <div class="hidden md:flex justify-center">
    <img class="h-full" alt="college graduate" src="/whycoaching.jpg" />
  </div>
</div>
<div class="bg-kbcblue w-full flex justify-center py-8">
  <div
    class="bg-white p-8 grid grid-cols-1 w-2/3 md:w-1/2 place-items-center text-kbcblue"
  >
    <h1 class="text-3xl font-bold">Success Story</h1>
    <p class="py-8 px-8">
      "Our practice session was extremely helpful for me in getting familiar
      with interview questions. Almost everything we discussed was asked in some
      way or form in the actual interview."
    </p>
    <h2 class="font-bold text-xl">
      <i>- Nick Horst, University of MN Student</i>
    </h2>
  </div>
</div>

<div
  class="bg-[url('/tip90.jpg')] bg-no-repeat bg-cover bg-center w-full py-16 flex justify-center"
>
  <div
    class="bg-white w-2/3 md:w-1/2 p-8 grid grid-cols-1 place-items-center text-kbcblue"
  >
    <h1 class="text-3xl font-bold">TIP #90...as in 90 SECONDS</h1>
    <p class="p-4">
      That's the average time it takes for hiring managers to know if they'd
      hire a candidate. Let's make that time count!
    </p>
  </div>
</div>

<div
  class="bg-white w-full grid grid-cols-1 place-items-center p-16 text-kbcblue"
>
  <h1 class="font-bold text-3xl pb-8">Two Ways to Meet:</h1>
  <div class="flex flex-col md:flex-row justify-center items-start">
    <div class="flex-1 grid grid-cols-1 place-items-center">
      <img
        src={base + "/homeoffice.jpg"}
        alt="Meeting an interview candidate at my home office"
        class="w-1/2"
      />
      <h2 class="text-xl font-bold py-4">My Home Office</h2>
      <p class="text-center pb-12">
        If you're in the Twin Cities, let's meet in person.
      </p>
    </div>
    <div class="flex-1 grid grid-cols-1 place-items-center">
      <img
        src={base + "/virtualinterview.jpg"}
        alt="Meeting an interview candidate over Zoom"
        class="w-1/2"
      />
      <h2 class="text-xl font-bold py-4">Virtual Meetings</h2>
      <p class="text-center pb-12">
        If you're out of town or want to practice virtual interviewing.
      </p>
    </div>
  </div>
</div>
