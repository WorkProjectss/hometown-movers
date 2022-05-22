<script setup>
</script>

<template>
  <header class="absolute z-10 top-0 w-screen flex items-center justify-between px-10 py-5 bg-gradient-to-b from-[#21201c]/50 to-transparent">
    <img class="w-[150px] brightness-0 invert" src="./assets/HometownFNL.png"/>
    <div class="flex gap-4">
      <a class="font-bold" href="#/about">HOME</a>
      <a class="font-bold" href="#/about">SERVICES</a>
      <a class="font-bold" href="#/about">ABOUT US</a>
      <a class="font-bold" href="#/about">CONTACT</a>
    </div>
  </header>
  <main class="relative h-screen w-screen overflow-hidden">
      <video 
        src="./assets/video-bg.m4v"
        autoplay
        muted
        loop
        class="min-h-full min-w-[100vw] w-auto h-auto"

      />
    <Button class="absolute left-[50%] -translate-x-[50%] bottom-10 text-[#21201c] bg-[#f69c22] py-2 px-4 rounded-2xl text-3xl font-bold ">
      CALL TO BOOK TODAY!
    </Button>
  </main>
  
  <section class="w-screen flex flex-col items-center bg-[#21201c] px-8 py-4">
    <div class="flex gap-2 mb-2">
      <svg v-for="i in 5" :key="i" class="w-5" viewBox="0 0 80 76" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M40 61.08L64.72 76L58.16 47.88L80 28.96L51.24 26.52L40 0L28.76 26.52L0 28.96L21.84 47.88L15.28 76L40 61.08Z" fill="#f69c22"/>
      </svg>
    </div>
    <p class="text-center font-medium">Austin and his team provided me with 5-star service. I am very pleased with their professionalism, courtesy, and efficiency. Hometown Movers got the job completed quickly and went above my expectaions. Thank you gentelmen. Y'all did a great job!</p>
    <p>- Rocky</p>
    <!-- facebook reviews -->
  </section>
  
  <section class="w-screen pt-5">
    <h2 class="w-full text-center text-[#f69c22] text-5xl font-[#21201c]  font-black py-2 mb-4">SERVICES</h2>
    <div class="flex justify-center gap-5 px-5 w-full font-bold">
      <div class="relative bg-[#21201c] min-w-[23%] h-[75vh]">
        <img class="absolute h-full w-auto -translate-x-1 -translate-y-1" src="./assets/residential-service.jpeg" />
        <p class="absolute bottom-4 left-[50%] -translate-x-[50%] text-3xl font-[#21201c] text-[#f69c22]">RESIDENTIAL</p>
      </div>
      <div class="relative bg-[#21201c] min-w-[23%] h-[75vh]">
        <img class="absolute h-full w-auto -translate-x-1 -translate-y-1" src="./assets/commercial-service.jpeg" />
        <p class="absolute bottom-4 left-[50%] -translate-x-[50%] text-3xl font-[#21201c] text-[#f69c22]">COMMERCIAL</p>
      </div>
      <div class="relative bg-[#21201c] min-w-[23%] h-[75vh]">
        <img class="absolute h-full w-auto -translate-x-1 -translate-y-1" src="./assets/local-service.jpeg" />
        <p class="absolute bottom-4 left-[50%] -translate-x-[50%] w-full text-center text-3xl font-[#21201c] text-[#f69c22]">LOCAL & LONG DISTANCE</p>
      </div>
      <div class="relative bg-[#21201c] min-w-[23%] h-[75vh]">
        <img class="absolute h-full w-auto -translate-x-1 -translate-y-1" src="./assets/storage-service.jpeg" />
        <p class="absolute bottom-4 left-[50%] -translate-x-[50%] text-3xl font-[#21201c] text-[#f69c22]">STORAGE</p>
      </div>

    </div>
  </section>

  <section class="w-screen pt-5 mb-10">
    <h2 class="w-full text-center text-[#f69c22] text-5xl font-[#21201c]  font-bold py-2">ABOUT HOMETOWN</h2>
    <div class="bg-[#f69c22] py-2 px-8 text-lg">
      <p class="text-center text-[#21201c] font-medium">Here at Hometown Movers LLC, we take pride in our work and customer satisfaction. Since being established in 2017, we have professionally moved thousands of families from one hometown to the next. We are a fully licensed and insured moving company that is locally owned and based in Godley, Texas. Call today and let us be a part of your new Hometown!</p>
    </div>
  </section>

  <section class="w-screen pt-5 mb-10">
    <h2 class="w-full text-center text-[#f69c22] text-5xl font-[#21201c] font-black py-2">ABOUT THE OWNERS</h2>
    <div class="flex">
    <img 
      src="./assets/moversabout.jpeg"
      class="max-w-[50%]"
    />
    <div class="bg-[#21201c] flex items-center justify-center">
     <p class="text-[#f69c22] font-medium text-lg text-center px-10">Hometown Movers was established in 2017 by Riley Davis and Austin Martinez, two entrepreneurs and best friends who grew up together in Godley, Texas. Growing up, the pair played along side each other on many athletic teams and knew they wanted to create a business together in the future. Their athletic backgrounds proved beneficial because they knew they had each others back and now run Hometown Movers with a team mindset. Being from Godley, the two men enjoy seeing their hometown grow and are proud to play their part in doing so</p> 
    </div>
    </div>
  </section>
  <section>
    <h2 class="w-full text-center text-[#f69c22] text-5xl font-[#21201c] font-black py-2">CONTACT</h2>
    <div class="text-[#21201c] flex items-center justify-between">
      <div class="w-1/2 flex flex-col items-center">
        <img class="w-[120px]" src="./assets/fb-logo.png"/>
        <p class="text-4xl w-[60%] text-center font-medium">
        CHECK US OUT ON FACEBOOK!
        </p>
      </div>
        <hr class="w-1 h-[240px] bg-[#f69c22]">
      <div class="w-1/2 flex flex-col items-center pl-20 gap-2">
        <p class="text-4xl w-[70%] text-center font-medium">CALL TO BOOK YOUR MOVE TODAY</p>
        <p class="text-5xl w-[60%] text-center font-[#21201c] font-bold">817.240.2061</p>
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
#app{
  font-family: 'futura';
  width:100vw;
  color:white;
}
</style>
