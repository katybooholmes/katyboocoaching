<script lang="ts">
  import { base } from "$app/paths";
  import Navbar from "$lib/Navbar.svelte";

  import SvgIcon from "@jamescoyle/svelte-icon";
  import {
    mdiFileCertificate,
    mdiPencilBoxMultiple,
    mdiStrategy,
    mdiCheckCircle,
    mdiCheckBold,
  } from "@mdi/js";

  let mdiType = "mdi";
  const areasOfFocus = [
    {
      label: "Visual Impact",
      img: mdiFileCertificate,
      list: ["Layout", "Branding", "Enhancements"],
    },
    {
      label: "Writing Quality",
      img: mdiPencilBoxMultiple,
      list: [
        "Clichés/overworked phrases",
        "Punctuation",
        "Verb tense and voice",
        "Clarity, word choice",
        "Rhythm and flow",
        "Brevity/concise writing",
        "Redundancies",
        "Adjective/adverb overload",
      ],
    },
    {
      label: "Strategy",
      img: mdiStrategy,
      list: [
        "Target/goal",
        "Industry/employer needs—Hard skills",
        "Soft skills/behavioral strengths",
        "Distinguishing information",
        "Tone/writing style",
        "Design/image",
      ],
    },
  ];

  const checkMarks = [
    { label: "Send me your resume for review" },
    {
      label: "We'll set a time to discuss:",
      list: [
        "your ideal job",
        "target industries",
        "experience",
        "transferrable skills",
        "results and added value, not just listing jobs/dates",
      ],
    },
    {
      label:
        "I will recreate your resume qualifying your experiences. I'll return for your review, edits",
    },
  ];
</script>

<Navbar currLoc={"/resume"} />

<div class="w-full bg-white grid grid-cols-1 place-items-center p-16">
  <div class="w-2/3 grid grid-cols-1 place-items-center">
    <h1 class="text-xl px-2">
      Together we can write a resume that <b>shows</b> not just <b>tells</b>.
    </h1>
    <img
      class="py-8 px-2"
      src={base + "/resumehead.jpg"}
      alt="seated interview candidates"
    />
  </div>
  <ul class="text-left list-disc w-1/2 py-8 border-kbcgold border-y-2">
    <li>
      Our goal is to write meaningful content that previews your potential
    </li>
    <li>Keep it tight but make it keyword rich</li>
    <li>Make it visually appealing but ATS friendly</li>
    <li>Target a broad audience and customize per opportunity</li>
  </ul>
  <div>
    <h2 class="font-bold text-2xl py-4 underline">Your resume should</h2>
    <ul class="list-none ">
      <li class="flex flex-row p-1">
        <SvgIcon class="pb-1" type={mdiType} path={mdiCheckBold} />Capture
        Attention
      </li>
      <li class="flex flex-row p-1">
        <SvgIcon class="pb-1" type={mdiType} path={mdiCheckBold} />
        Generate Interest
      </li>
      <li class="flex flex-row p-1">
        <SvgIcon class="pb-1" type={mdiType} path={mdiCheckBold} />
        Cultivate Desire
      </li>
      <li class="flex flex-row p-1">
        <SvgIcon class="pb-1" type={mdiType} path={mdiCheckBold} />
        Inspire Action
      </li>
    </ul>
  </div>
</div>
<div class="w-full bg-kbcgold py-16 flex justify-center">
  <div>
    <h1 class="text-3xl font-bold pb-8 text-center">
      We have 3 primary areas of focus
    </h1>
    <div
      class="flex flex-col sm:flex-row sm::justify-center sm:items-start gap-16"
    >
      {#each areasOfFocus as area}
        <div class="flex-1 grid grid-cols-1 place-items-center">
          <SvgIcon size="72" type={mdiType} path={area.img} />
          <h2 class="font-bold uppercase">{area.label}</h2>
          <ul class="list-disc py-2">
            {#each area.list as item}
              <li>{item}</li>
            {/each}
          </ul>
        </div>
      {/each}
    </div>
  </div>
</div>
<div class="w-full bg-white p-8 grid grid-cols-1 place-items-center">
  <img
    class="sm:w-1/2 md:w-1/4"
    src={base + "/resumelaptop.jpg"}
    alt="a laptop writing a resume"
  />
  <div
    class="flex flex-col sm:flex-row sm::justify-center sm:items-start gap-8 py-4"
  >
    {#each checkMarks as checkmark}
      <div class="flex-1 grid grid-cols-1 place-items-center text-center">
        <SvgIcon
          class="text-kbcgold"
          size="72"
          type={mdiType}
          path={mdiCheckCircle}
        />
        <h2>{checkmark.label}</h2>
        {#if checkmark.list != undefined}
          <ul class="list-disc text-left pl-4 pt-4">
            {#each checkmark.list as listitem}
              <li>{listitem}</li>
            {/each}
          </ul>
        {/if}
      </div>
    {/each}
  </div>
  <h2 class="py-8 text-6xl font-light">$149</h2>
  <button
    class="py-2 px-16 bg-white font-bold text-black border border-black border-1 hover:bg-black hover:text-white"
    >Sign me up</button
  >
</div>
