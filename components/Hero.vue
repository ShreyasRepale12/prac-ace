<template>
  <div style="background-color: #001e26" class="pt-20">
    <div class="container mx-auto flex flex-col items-center py-14 sm:py-24">
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
            transition
            duration-150
            ease-in-out
            text-white
            hover:bg-green-600
            rounded-full
            text-white
            px-8
            sm:px-12
            py-1
            sm:py-2
            text-lg
            bg-gradient-to-r
            from-green-400
            to-blue-500
            hover:from-pink-500 hover:to-yellow-500
            font-semibold
          "
          style="background-color: #4ce6a7"
        >
          Join Club
        </button>
        <button
          class="
            ml-4
            focus:outline-none
            bg-white
            transition
            duration-150
            ease-in-out
            hover:border-indigo-600 hover:text-gray-900 hover:bg-green-400
            rounded-full
            border border-indigo-700
            text-indigo-700
            px-4
            sm:px-10
            py-1
            sm:py-2
            text-lg
            font-semibold
          "
        >
          Learn More
        </button>
      </div>
      <img
        src="~/static/hero-logos/vue-logo.png"
        alt="VueJs"
        style="
          position: absolute;
          width: 80px;
          height: 80px;
          top: 90px;
          right: 190px;
          transform: rotate(20deg);
        "
        id="content-desktop"
      />
      <img
        src="~/static/hero-logos/kotlin-logo.png"
        alt="Kotlin"
        style="
          position: absolute;
          width: 90px;
          height: 90px;
          top: 130px;
          left: 120px;
          transform: rotate(20deg);
        "
        id="content-desktop"
      />

      <img
        src="~/static/hero-logos/react-logo.png"
        alt="ReactJS"
        style="
          position: absolute;
          width: 90px;
          height: 90px;
          top: 430px;
          left: 180px;
        "
        id="content-desktop"
      />
    </div>

    <img
      src="~/static/hero-logos/angular-logo.png"
      alt="Angular"
      style="
        position: absolute;
        width: 80px;
        height: 80px;
        top: 490px;
        right: 240px;
        transform: rotate(-10deg);
      "
      id="content-desktop"
    />
    <div
      style="height: 160px"
      class="invisible md:visible" id="content-desktop"
    ></div>
    <img src="~/static/cheer.gif" id="content-mobile" style="width: 100px; height: 100px;" class="container mx-auto flex flex-col items-center pb-3">
  </div>
</template>

<script>
export default {
  name: "Hero",
  mounted() {
  },
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

#content-desktop {
  display: block;
}
#content-mobile {
  display: none;
}

@media screen and (max-width: 768px) {
  #content-desktop {
    display: none;
  }
  #content-mobile {
    display: block;
  }
}
</style>