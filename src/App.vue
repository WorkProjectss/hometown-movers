<script setup>
import { ref } from 'vue';
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';

  const reviews = ref([
  {
    reviewerName:'Jake Tolbert',
    review:"I've used them twice now, always on time or 15 minutes early. Extremely professional movers that I will definitely use again!",
  },
  {
    reviewerName:"Robin Rowe Kiel",
    review:"Very professional, friendly and fantastic job ! Packed up our house of 27 years and moved us to new place with a smile in record time. They are the BEST !!!"
  },
  {
    reviewerName:'Robin K Nan Marie Gauthier',
    review:"Hometown Movers did an excellent & quick job loading our third floor apartment (without an elevator) into our moving truck! No damages, super friendly, on time, & super efficient! I highly recommend this team for your next move!"
  },
  {
    reviewerName:'Tami Golightly',
    review:"If you're moving soon you NEED to contact these guys. I highly recommend them!! They moved us from Burleson to Godley & did it in less time than they quoted us. They we're so much fun to work with & really take pride in what they do! They even let my 12 yo help out & let my 8yo honk the horn in their big truck!"
  },
  {
    reviewerName:'Rocky',
    review:"Austin and his team provided me with 5-star service. I am very pleased with their professionalism, courtesy, and efficiency. Hometown Movers got the job completed quickly and went above my expectaions. Thank you gentelmen. Y'all did a great job!"
  }

])
</script>

<template>
  <main class="relative md:h-screen w-screen overflow-hidden">
  <header class="absolute z-10 top-0 w-screen flex items-center justify-between md:px-10 px-5 py-5 bg-gradient-to-b from-[#21201c]/50 to-transparent">
    <img class="md:w-[250px] w-[280px] brightness-0 invert absolute md:relative left-[50%] -translate-x-[50%] md:transform-none md:inset-0 sm:top-[40vh] top-[22vh]" src="./assets/HometownFNL.png"/>
    <div class="flex gap-4 md:w-auto items-center justify-center w-screen">
      <a class="font-bold text-sm md:text-xl" href="#">HOME</a>
      <a class="font-bold text-sm md:text-xl" href="#services">SERVICES</a>
      <a class="font-bold text-sm md:text-xl" href="#about">ABOUT US</a>
      <a class="font-bold text-sm md:text-xl" href="#contact">CONTACT</a>
    </div>
  </header>
      <video 
        src="./assets/videobg.mp4"
        autoplay
        muted
        loop
        playsinline
        class="lg:w-[105vw] xl:w-[120vw] md:w-[140vw] w-[200vw]"
      />
    <a href="tel:+1 817-240-2061" class="absolute left-[50%] z-20 -translate-x-[50%] md:bottom-10 bottom-2 md:w-auto  w-[85%] text-[#21201c] bg-[#f69c22] py-4 px-8 rounded-3xl md:text-5xl text-xl font-bold text-center">
      CALL TO BOOK TODAY!
    </a>
  </main> 
  <section class="w-screen flex gap-2 justify-evenly px-8 pt-2 bg-[#21201c] max-w-[100vw] overflow-hidden">
  <carousel :autoplay="10000" :transition="1500" :wrapAround="true" :items-to-show="1">
    <slide v-for="review in reviews" :key="review.reviewerName"  >
<div class="h-full flex flex-col items-center justify-evenly">
      <p class="text-center font-bold lg:font-medium md:text-4xl bg-orange-400/50 w-[40px] lg:w-[60px] lg:h-[60px] p-2 rounded-full">{{review.reviewerName[0]}}</p>
      <p class="text-center font-medium md:text-xl lg:w-[50%] w-[50%]">{{review.review}}</p>
      <div class="flex gap-2 mb-2 mt-2">
      <svg v-for="i in 5" :key="i" class="w-5" viewBox="0 0 80 76" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M40 61.08L64.72 76L58.16 47.88L80 28.96L51.24 26.52L40 0L28.76 26.52L0 28.96L21.84 47.88L15.28 76L40 61.08Z" fill="#f69c22"/>
      </svg>
      </div>
      <p class="md:text-xl">- {{review.reviewerName}}</p>
      </div>
    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>
    <!-- facebook reviews -->
  </section>
  
  <section class="w-screen pt-5" id="services">
    <h2 class="w-full text-center text-[#f69c22] md:text-5xl text-3xl font-[#21201c]  font-black py-2 mb-4">SERVICES</h2>
    <div class="grid lg:grid-cols-4 sm:grid-cols-2 grid-cols-1 justify-center gap-5 px-5 w-full font-bold">
      <div class="relative bg-[#21201c] min-w-[23%] h-[70.5vh]">
        <img class="absolute object-cover h-full w-full -translate-x-1 -translate-y-1" src="./assets/residential-service.jpeg" />
        <p class="absolute bottom-4 left-[50%] -translate-x-[50%]  md:text-3xl text-xl font-[#21201c] text-[#f69c22]">RESIDENTIAL</p>
      </div>
      <div class="relative bg-[#21201c] min-w-[23%] h-[70.5vh]">
        <img class="absolute object-cover h-full w-full -translate-x-1 -translate-y-1" src="./assets/commercial-service.jpeg" />
        <p class="absolute bottom-4 left-[50%] -translate-x-[50%]  md:text-3xl text-xl font-[#21201c] text-[#f69c22]">COMMERCIAL</p>
      </div>
      <div class="relative bg-[#21201c] min-w-[23%] h-[70.5vh]">
        <img class="absolute object-cover h-full w-full -translate-x-1 -translate-y-1" src="./assets/local-service.jpeg" />
        <p class="absolute bottom-4 left-[50%] -translate-x-[50%] w-full text-center  md:text-3xl text-xl font-[#21201c] text-[#f69c22]">LOCAL & LONG DISTANCE</p>
      </div>
      <div class="relative bg-[#21201c] min-w-[23%] h-[70.5vh]">
        <img class="absolute object-cover h-full w-full -translate-x-1 -translate-y-1" src="./assets/storage-service.jpeg" />
        <p class="absolute bottom-4 left-[50%] -translate-x-[50%] md:text-3xl text-xl font-[#21201c] text-[#f69c22]">STORAGE</p>
      </div>

    </div>
  </section>

  <section class="w-screen pt-5 md:mb-2 mt-16 md:mt-0" id='about'>
    <h2 class="w-full text-center text-[#f69c22]  md:text-5xl text-3xl font-[#21201c]  font-bold py-2">ABOUT HOMETOWN</h2>
    <div class="bg-[#f69c22] py-2 px-8 text-lg">
      <p class="text-center text-[#21201c] font-medium md:text-2xl 2xl:text-4xl">Here at Hometown Movers LLC, we take pride in our work and customer satisfaction. Since being established in 2017, we have professionally moved thousands of families from one hometown to the next. We are a fully licensed and insured moving company that is locally owned and based in Godley, Texas. Call today and let us be a part of your new Hometown!</p>
    </div>
  </section>

  <section class="w-screen pt-5 mb-5">
    <h2 class="w-full text-center text-[#f69c22] md:text-5xl text-3xl  font-[#21201c] font-black py-2">ABOUT THE OWNERS</h2>
    <div class="flex md:flex-row flex-col">
    <img 
      src="./assets/moversabout.jpeg"
      class="md:max-w-[50%] max-w-[100%] object-cover"
    />
    <div class="bg-[#21201c] flex items-center justify-center">
     <p class="text-[#f69c22] font-medium text-lg text-center px-10 md:text-2xl 2xl:text-3xl py-4 lg:py-0">Hometown Movers was established in 2017 by Riley Davis and Austin Martinez, two entrepreneurs and best friends who grew up together in Godley, Texas. Growing up, the pair played along side each other on many athletic teams and knew they wanted to create a business together in the future. Their athletic backgrounds proved beneficial because they knew they had each others back and now run Hometown Movers with a team mindset. Being from Godley, the two men enjoy seeing their hometown grow and are proud to play their part in doing so!</p> 
    </div>
    </div>
  </section>
  <section id='contact'>
    <h2 class="w-full text-center text-[#f69c22] md:text-5xl text-3xl  font-[#21201c] font-black py-2">CONTACT</h2>
    <div class="text-[#21201c] flex flex-col md:flex-row items-center justify-between gap-4 md:gap-0">
      <div class="w-1/2 flex flex-col items-center gap-2 md:gap-0">
        <img class="w-[120px]" src="./assets/fb-logo.png"/>
        <a href="https://web.facebook.com/hometownmovers223/" target="_blank" class="md:text-4xl text-xl 2xl:text-7xl md:w-[60%] w-[100%] text-center font-medium">
        CHECK US OUT ON FACEBOOK!
        </a>
      </div>
        <hr class="md:w-1 md:h-[240px] w-[300px] h-1 bg-[#f69c22]">
      <div class="md:w-1/2 w-full flex flex-col items-center md:pl-20 gap-2">
        <p class="md:text-4xl 2xl:text-7xl text-xl md:w-[70%] w-[60%] text-center font-medium">CALL TO BOOK YOUR MOVE TODAY</p>
        <p class="md:text-5xl 2xl:text-7xl text-2xl w-[60%] text-center font-[#21201c] font-bold">817.240.2061</p>
      </div>
    </div>
  </section>
  <p class="w-screen text-center text-[#21201c] my-4">&copy; Hometown Movers.All rights reserved. Hometown Movers</p>
</template>

<style>
@font-face {
  font-family: "futura";
  src:  url("./assets/font/futur.ttf") format("truetype");
  font-weight:normal;
  font-style:normal;
}

@font-face {
  font-family: "futura";
  src:  url("./assets/font/futura medium bt.ttf") format("truetype");
  font-weight:medium;
  font-style:normal;
}

@font-face {
  font-family: "futura";
  src:  url("./assets/font/unicode.futurab.ttf") format("truetype");
  font-weight:bold;
  font-style:normal;
}
html{
  overflow-x:hidden;
}
video{
  max-width: initial !important;
}
#app{
  font-family: 'futura';
  width:100vw;
  color:white;
}
</style>
