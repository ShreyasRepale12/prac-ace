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
        src="~/static/ruby.png"
        alt="Ruby"
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
        alt="Ruby 1"
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
    
      <img src="~/static/ruby2.png" class="rubydesktop" style="
          position: absolute;
          top: 450px;
          left: 10px;
        " id="content-desktop">

      <img src="~/static/ruby2.png" class="rubymobile" height="75px" width="75px" style="position: absolute;
          top: 400px;
          left: 10px;" id="content-mobile">
    <br><br><br><br><br><br><br><br><br><br><br><br>
  </div>
</template>

<script>
export default {
  name: "Hero",
  mounted() {
    this.animateOnScroll();
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
    animateOnScroll() {
      this.$gsap.to(".rubydesktop", {
      rotation: 480,
      x: 850,
      duration: 5
    });
    this.$gsap.to(".rubymobile", {
      rotation: 480,
      x: 150,
      duration: 5
    });
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