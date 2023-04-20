<script lang="ts">
  import Navbar from "$lib/Navbar.svelte";
  import SvgIcon from "@jamescoyle/svelte-icon";
  import {
    mdiEyeOutline,
    mdiAccountTie,
    mdiMessageReply,
    mdiInformationVariantBoxOutline,
    mdiHelpCircle,
    mdiHandshakeOutline,
  } from "@mdi/js";

  const pictograms = [
    { label: "First Impressions", img: mdiEyeOutline },
    { label: "Non-verbal Communication", img: mdiAccountTie },
    { label: "Your Key Messages", img: mdiMessageReply },
    { label: "Transferrable Skills", img: mdiInformationVariantBoxOutline },
    { label: "Elevator Speech", img: mdiHelpCircle },
    { label: "After the Interview", img: mdiHandshakeOutline },
  ];
</script>

<Navbar currLoc={"/how"} />

<div
  class="w-full bg-[url('/howheader.jpg')] bg-no-repeat bg-cover bg-bottom py-64 text-center text-white text-6xl font-bold"
>
  Let's Work Together
</div>
<div class="w-full py-8 bg-white grid grid-cols-1 place-items-center">
  <div class="w-1/2 grid grid-cols-1 gap-4 py-8">
    <p>
      The goal of personalized interview coaching is to build confidence through
      practice. You may think you don't have enough experience or the right
      qualifications but that's where coaching can help you dig deeper and
      identify your accomplishments as examples of transferrable skills, like
      teamwork, organization, or problem-solving.
    </p>
    <p>
      You will learn what to expect in a job interview and to think on your
      feet. You'll have strong answers—prepared but not memorized—no matter what
      questions are asked.
    </p>
  </div>
  <div class=" grid grid-cols-1 place-items-center">
    <h1 class="font-bold text-3xl py-8">We'll cover</h1>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-16 pb-8">
      {#each pictograms as pictogram}
        <div class="grid grid-cols-1 place-items-center">
          <SvgIcon
            class="text-kbcgold"
            size="120"
            type={"mdi"}
            path={pictogram.img}
          />
          <h2 class="text-center text-xl font-bold">{pictogram.label}</h2>
        </div>
      {/each}
    </div>
  </div>
</div>
<div
  class="w-full bg-[url('/tip210.jpg')] bg-no-repeat bg-cover py-32 flex justify-center"
>
  <div class="py-8 bg-white w-1/2 text-center">
    <h1 class="font-bold text-3xl pb-2">TIP #210</h1>
    <p class="px-8">
      Hiring managers say one of their biggest pet peeves is interviewees who
      talk too much. Let's work on complete but brief answers.
    </p>
  </div>
</div>
<div
  class="w-full bg-white grid grid-cols-1 place-content-center text-center px-8 md:px-32 py-16"
>
  <h1 class="font-bold text-4xl">Cost</h1>
  <div class="flex flex-col p-8 gap-4 md:flex-row">
    <div class="bg-stone-200 p-8 flex-1 grid grid-cols-1 place-items-center">
      <h3 class="font-bold text-xl">Starting Blocks</h3>
      <p class="py-8">
        Coaching service is $149 for 60-minute session with mock interview and
        preliminary homework
      </p>
      <ul class="list-disc text-left">
        <li>Preparing for specific aspects of the interview</li>
        <li>Conducting a mock interview</li>
        <li>Immediate feedback</li>
        <li>Available Virtually or In-Person</li>
      </ul>
      <h3 class="font-bold text-lg py-8">$149</h3>
    </div>
    <div class="bg-stone-200 p-8 flex-1 grid grid-cols-1 place-items-center">
      <h3 class="font-bold text-xl">Pace Setter</h3>
      <p class="py-8">Additional 60-minute sessions could include:</p>
      <ul class="list-disc text-left">
        <li>Additional review of interview answers</li>
        <li>Second-round mock interview</li>
        <li>Other issues/questions you want to cover</li>
        <li>Available Virtually or In-Person</li>
      </ul>
      <h3 class="font-bold text-lg py-8">$100/session</h3>
    </div>
  </div>
</div>
<div class="w-full bg-kbcgold py-16 flex justify-center">
  <div class="bg-white w-1/2 p-8 text-center">
    <h1 class="font-bold text-3xl pb-2">TIP #47</h1>
    <p>
      The dreaded "Where do you want to be in 5 years?" question. Let's work on
      your sincere answer.
    </p>
  </div>
</div>
