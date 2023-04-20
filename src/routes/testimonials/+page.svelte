<script lang="ts">
  import Navbar from "$lib/Navbar.svelte";

  const testimonials = [
    {
      text: "I really appreciate that, while I did my research and preparation, Katy also did hers. So we were able to bring both sets of knowledge of the med school interview to the table and collaborate. Katy also provided great feedback in the moment.",
      saidBy: "Elizabeth Pryor, Med School Candidate",
    },
    {
      text: "Katy coached a class of high schoolers and she took the mystery out of what happens in an interview by walking students through the specific stages. Katy helped make the process more transparent, by cluing them into all of the non-verbal communication that occurs.",
      saidBy: "Janet Schmiel, Edina High School Counselor",
    },
    {
      text: "Katy helped my daughter prepare for her first job interview. Together they discussed my daughter's strengths and talents, as well as her hobbies and extra-curriculars, as a way to show leadership and perseverance. It was really helpful for my daughter to get a practice interview before the real thing. It really boosted her confidence.",
      saidBy: "Kris Mollison, Parent",
    },
    {
      text: "Our practice session was extremely helpful for me in getting familiar with interview questions. Almost everything we discussed was asked in some way or form in the actual interview.",
      saidBy: "Nick Horst, University of MN Student",
    },
  ];
</script>

<Navbar currLoc={"/testimonials"} />

<div
  class="w-full bg-[url('/testimonialsheader.jpg')] bg-cover bg-no-repeat py-32 text-3xl text-white font-bold text-center"
/>

<div class="w-full bg-kbcgold p-4 py-8 grid grid-cols-1 place-items-center">
  <h1 class="text-3xl font-bold pb-8">Testimonials</h1>
  <div
    class="md:w-2/3 grid grid-cols-1 md:grid-cols-2 place-content-center gap-8"
  >
    {#each testimonials as test}<div>
        <p>"{test.text}"</p>
        <h3 class="text-center py-2 italic text-sm">-{test.saidBy}</h3>
      </div>{/each}
  </div>
  <div class="bg-white w-2/3 py-8 my-16 text-center">
    <h2 class="pb-2 font-bold text-3xl">TIP #168</h2>
    <p class="px-8">
      The average corporate job attracts <b>250</b> resumes, which leads to
      <b>4-6</b>
      interviews, for <b>1</b> job. Crush the interview, land the job.
    </p>
  </div>
</div>
