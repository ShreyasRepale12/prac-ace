<template>
  <div style="background-color: #001e26" class="pt-10">
    <div class="container mx-auto flex flex-col items-center py-12 sm:py-24">
      <div class="w-11/12 sm:w-2/3 mb-5 sm:mb-10">
        <h1
          class="
            text-4xl
            sm:text-5xl
            md:text-5xl
            lg:text-6xl
            xl:text-7xl
            text-center text-white
            leading-tight
          "
          style="font-family: 'DM Serif Display', serif"
        >
          We Are Association of Coders and Encoders Club
        </h1>
        <p
          class="
            mt-3
            sm:mt-8
            pt-2
            text-gray-400
            font-normal
            text-center text-xl
            sm:text-2xl
          "
        >
          Develop Your Skills, Learn Something New, and Grow Your Skills With
          Association of Coders and Encoders.
        </p>
      </div>
      <div class="flex justify-center items-center">
        <button
          class="
            focus:outline-none
            bg-indigo-700
            transition
            duration-150
            ease-in-out
            hover:bg-indigo-600
            rounded
            text-white
            px-4
            sm:px-10
            py-2
            sm:py-4
            text-sm
          "
        >
          Get Started
        </button>
        <button
          class="
            ml-4
            focus:outline-none
            bg-white
            transition
            duration-150
            ease-in-out
            hover:border-indigo-600 hover:text-indigo-600
            rounded
            border border-indigo-700
            text-indigo-700
            px-4
            sm:px-10
            py-2
            sm:py-4
            text-sm
          "
        >
          Live Demo
        </button>
      </div>
      <img
        src="~/static/ruby.png"
        alt="Smiley face"
        style="
          position: absolute;
          width: 100px;
          height: 100px;
          top: 80px;
          right: 190px;
        "
        id="content-desktop"
      />
      <img
        src="~/static/ruby2.png"
        alt="Smiley face"
        style="
          position: absolute;
          width: 200px;
          height: 200px;
          top: 130px;
          right: 1200px;
        "
        id="content-desktop"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "CentreAlignedSimple",
  methods: {
    // Function to toggle header menu in mobile view.
    toggleMenu(flag) {
      let value = document.getElementById("menu");
      if (flag) {
        value.classList.remove("hidden");
      } else {
        value.classList.add("hidden");
      }
    },
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=DM+Serif+Display&display=swap");

#content-desktop {display: block;}
#content-mobile {display: none;}

@media screen and (max-width: 768px) {

#content-desktop {display: none;}
#content-mobile {display: block;}

}
</style>