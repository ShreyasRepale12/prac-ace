<template>
  <div
    class="pt-5 container mx-auto flex flex-col items-center p-4"
    style="background-color: #e5f9ff"
  >
    <h1
      class="
        eventsheading
        font-medium
        leading-tight
        sm:text-5xl
        text-3xl
        pt-6
        mb-6
        text-gray-900
      "
      style="font-family: 'DM Serif Display', serif"
    >
      Fe<span style="color: #00db80">a</span>ture Even<span
        style="color: #00db80"
        >t</span
      >s
    </h1>

    <div class="grid grid-cols-2 gap-8 md:gap-12">
      <a
        href="#"
        class="
          flex flex-col
          items-center
          rounded-lg
          border
          shadow-md
          md:flex-row md:max-w-xl
          hover:bg-dark
          lg:col-span-1
          col-span-2
        "
        style="background-color: #001e26;"
      >
        <img
          class="
            object-cover
            w-full
            h-96
            rounded-t-lg
            md:h-auto md:w-48 md:rounded-none md:rounded-l-lg
          "
          src="https://venngage-wordpress.s3.amazonaws.com/uploads/2018/11/Blue-Pool-Party-Creative-Poster-Example2.jpg"
          alt=""
        />
        <div class="flex flex-col justify-between p-4 leading-normal">
          <h5
            class="
              mb-2
              text-2xl
              font-bold
              tracking-tight
              text-white
            "
          >
            Master Git and Github from Scratch
          </h5>
          <p class="mb-3 font-normal text-gray-300">
            Here are the biggest enterprise technology acquisitions of 2021 so
            far, in reverse chronological order.
          </p>
        </div>
      </a>
      <a
        href="#"
        class="
          flex flex-col
          items-center
          bg-gray-900
          rounded-lg
          border
          shadow-md
          md:flex-row md:max-w-xl
          hover:bg-dark
          lg:col-span-1
          col-span-2
        "
      >
        <img
          class="
            object-cover
            w-full
            h-96
            rounded-t-lg
            md:h-auto md:w-48 md:rounded-none md:rounded-l-lg
          "
          src="https://www.washingtonpost.com/graphics/2019/entertainment/oscar-nominees-movie-poster-design/img/vice-web.jpg"
          alt=""
        />
        <div class="flex flex-col justify-between p-4 leading-normal">
          <h5
            class="
              mb-2
              text-2xl
              font-bold
              tracking-tight
              text-white
            "
          >
            Learn Core Java From Scratch
          </h5>
          <p class="mb-3 font-normal text-gray-300">
            Here are the biggest enterprise technology acquisitions of 2021 so
            far, in reverse chronological order.
          </p>
        </div>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    this.animateOnScroll();
  },
  methods: {
    animateOnScroll() {
      this.$gsap.to(".eventsheading", {
        x: 100,
        ease: "Power2.easeInOut",
        scrollTrigger: {
          trigger: "bottom",
          pin: true,
          end: "bottom 200px",
          scrub: true,
        },
      });
    },
  },
};
</script>

<style>
</style>