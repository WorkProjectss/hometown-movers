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
        src="./assets/Header.mp4"
        autoplay
        muted
        loop
        class="min-h-full min-w-[120vw] w-auto h-auto"

      />
    <Button class="absolute left-[50%] -translate-x-[50%] bottom-10 text-[#21201c] bg-[#f69c22] py-2 px-4 rounded-2xl text-3xl font-black ">
      CALL TO BOOK TODAY!
    </Button>
  </main>
  
  <section class="w-screen flex flex-col items-center bg-[#21201c] px-8 py-4">
    <div class="flex">
   <svg v-for="i in 5" :key="i" color="orange" xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
      <path  d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z" />
    </svg>
    </div>
    <p class="text-center">Austin and his team provided me with 5-star service. I am very pleased with their professionalism, courtesy, and efficiency. Hometown Movers got the job completed quickly and went above my expectaions. Thank you gentelmen. Y'all did a great job!</p>
    <p>- Rocky</p>
    <!-- facebook reviews -->
  </section>
  
  <section class="w-screen pt-5">
    <h2 class="w-full text-center text-[#f69c22] text-5xl font-[#21201c]  font-black py-2 mb-4">Services</h2>
    <div class="flex justify-center gap-5 px-5 w-full">
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
    <h2 class="w-full text-center text-[#f69c22] text-5xl font-[#21201c]  font-black py-2">ABOUT HOMETOWN</h2>
    <div class="bg-[#f69c22] py-2 px-8 text-lg">
      <p class="text-center text-[#21201c] font-medium">Hometown Movers was established in 2017 by Riley Davis and Austin Martinez, two entrepreneurs and best friends who grew up together in Godley, Texas. Growing up, the pair played along side each other on many athletic teams and knew they wanted to create a business together in the future. Their athletic backgrounds proved beneficial because they knew they had each others back and now run Hometown Movers with a team mindset. Being from Godley, the two men enjoy seeing their hometown grow and are proud to play their part in doing so</p>
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
        <svg width="43" height="43" viewBox="0 0 43 43" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M43 21.5C43 9.62677 33.3732 0 21.5 0C9.62677 0 0 9.62677 0 21.5C0 32.2303 7.86106 41.1254 18.1409 42.74V27.7163H12.6805V21.5H18.1409V16.7622C18.1409 11.3743 21.3518 8.39622 26.262 8.39622C28.6143 8.39622 31.0754 8.81648 31.0754 8.81648V14.1076H28.3633C25.6936 14.1076 24.8591 15.7644 24.8591 17.4667V21.5H30.8214L29.869 27.7163H24.8591V42.74C35.1389 41.1285 43 32.2334 43 21.5Z" fill="#1977F3"/>
          <path d="M29.8691 27.7163L30.8214 21.5H24.8591V17.4667C24.8591 15.7675 25.6906 14.1076 28.3634 14.1076H31.0754V8.8165C31.0754 8.8165 28.6143 8.39624 26.262 8.39624C21.3519 8.39624 18.141 11.3713 18.141 16.7622V21.5H12.6805V27.7163H18.141V42.74C19.2355 42.9123 20.3572 43 21.5 43C22.6429 43 23.7646 42.9093 24.8591 42.74V27.7163H29.8691Z" fill="#FEFEFE"/>
        </svg>
        <p class="text-4xl w-[60%] text-center font-medium">
        CHECK US OUT ON FACEBOOK!
        </p>
      </div>
        <hr class="w-1 h-[240px] bg-[#f69c22]">
      <div class="w-1/2 flex flex-col pl-20 gap-2">
        <p class="text-4xl w-[60%] text-center font-medium">CALL TO BOOK YOUR MOVE TODAY</p>
        <p class="text-5xl w-[60%] text-center font-[#21201c]">817.240.2061</p>
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
  src:  url("./assets/font/Futura Heavy font.ttf") format("truetype");
  font-weight:bold;
  font-style:normal;
}

html{
  overflow-x:hidden;
}
#app{
  width:100vw;
  color:white;
}
</style>
